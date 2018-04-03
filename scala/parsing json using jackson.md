import com.fasterxml.jackson.module.scala.DefaultScalaModule
import com.fasterxml.jackson.databind.ObjectMapper
import com.fasterxml.jackson.module.scala.experimental.ScalaObjectMapper

val objectMapper: ObjectMapper =  new ObjectMapper() with ScalaObjectMapper
objectMapper.registerModule(DefaultScalaModule)
val jsonMap: Map[String,Any] = objectMapper.readValue(json,classOf[Map[String,Any]])