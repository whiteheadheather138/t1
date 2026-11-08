代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：https://ea.zhonguo3118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://hw.zhonguo6118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://ii.zhonguo1118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://sg.zhonguo3118.cn

C#:   d1 < d2;  d1 == d2
来源：https://yc.zhonguo2118.cn

[J08] 提取年月日与星期
来源：https://ee.zhonguo3118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://oq.zhonguo6118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ho.zhonguo1118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://rm.zhonguo5118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://gx.zhonguo3118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://sm.zhonguo8118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://ql.zhonguo3118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://jx.zhonguo7118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://xl.zhonguo7118.cn

[J09] 时区处理
来源：https://nh.zhonguo6118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://ld.zhonguo6118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://lu.zhonguo4118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://oh.zhonguo6118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://cm.zhonguo3118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://yb.zhonguo4118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://ew.zhonguo2118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://zw.zhonguo5118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://yc.zhonguo2118.cn

[J10] 取今天 / 本月第一天
来源：https://tg.zhonguo8118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://gp.zhonguo4118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://vn.zhonguo4118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://hs.zhonguo4118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://bw.zhonguo8118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://mg.zhonguo8118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://dv.zhonguo1118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://vb.zhonguo8118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://wa.zhonguo5118.cn

================================================================================
来源：https://vf.zhonguo5118.cn

K. JSON 与序列化
来源：https://li.zhonguo3118.cn

================================================================================
来源：https://gl.zhonguo4118.cn

[K01] 对象转 JSON 字符串
来源：https://er.zhonguo4118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://wj.zhonguo1118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://fn.zhonguo4118.cn

JS:   JSON.stringify(obj)
来源：https://bf.zhonguo4118.cn

TS:   JSON.stringify(obj)
来源：https://jk.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://jj.zhonguo2118.cn

Go:   json.Marshal(obj)
来源：https://kn.zhonguo7118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://wf.zhonguo1118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://uj.zhonguo1118.cn

[K02] JSON 字符串转对象
来源：https://sb.zhonguo3118.cn

Py:   json.loads(s)
来源：https://qr.zhonguo6118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://ro.zhonguo2118.cn

JS:   JSON.parse(s)
来源：https://cr.zhonguo3118.cn

TS:   JSON.parse(s)
来源：https://qw.zhonguo4118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://zo.zhonguo2118.cn

Go:   json.Unmarshal(data, &v)
来源：https://ej.zhonguo3118.cn

Ruby: JSON.parse(s)
来源：https://mm.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://xj.zhonguo3118.cn

[K03] JSON 美化输出（带缩进）
来源：https://we.zhonguo6118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://wt.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://ep.zhonguo2118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://wj.zhonguo6118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://ey.zhonguo3118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://ts.zhonguo6118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://rq.zhonguo1118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://hf.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://bs.zhonguo8118.cn

[K04] 读取 JSON 文件
来源：https://aa.zhonguo4118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://lx.zhonguo8118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://ox.zhonguo4118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://yw.zhonguo8118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://aa.zhonguo7118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://vu.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://dp.zhonguo3118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://mg.zhonguo8118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://kx.zhonguo4118.cn

[K05] 深拷贝对象
来源：https://xb.zhonguo3118.cn

Py:   copy.deepcopy(obj)
来源：https://uh.zhonguo1118.cn

PHP:  unserialize(serialize($obj));
来源：https://jp.zhonguo5118.cn

JS:   structuredClone(obj)
来源：https://gc.zhonguo3118.cn

TS:   structuredClone(obj)
来源：https://eo.zhonguo7118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://yg.zhonguo3118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://qn.zhonguo7118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://cy.zhonguo3118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://ro.zhonguo3118.cn

[K06] 解析 URL 查询串
来源：https://me.zhonguo7118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://at.zhonguo8118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://fp.zhonguo3118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://bb.zhonguo3118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://kv.zhonguo2118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://uf.zhonguo2118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://nk.zhonguo4118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://yw.zhonguo5118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://zr.zhonguo8118.cn

[K07] 进制转换
来源：https://qe.zhonguo5118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://cg.zhonguo1118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://km.zhonguo3118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://mr.zhonguo5118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://kj.zhonguo2118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://ks.zhonguo8118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://yx.zhonguo4118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://cl.zhonguo4118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://ld.zhonguo5118.cn

[K08] 二进制序列化（非 JSON）
来源：https://pe.zhonguo6118.cn

Py:   pickle.dumps(obj)
来源：https://ky.zhonguo5118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://gv.zhonguo1118.cn

JS:   v8.serialize(obj)        // Node
来源：https://ob.zhonguo1118.cn

TS:   v8.serialize(obj)        // Node
来源：https://vp.zhonguo5118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://zk.zhonguo7118.cn

Go:   encoding/gob
来源：https://ut.zhonguo8118.cn

Ruby: Marshal.dump(obj)
来源：https://gy.zhonguo2118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://ey.zhonguo3118.cn

================================================================================
来源：https://ev.zhonguo8118.cn

L. 网络请求
来源：https://am.zhonguo3118.cn

================================================================================
来源：https://oo.zhonguo8118.cn

[L01] 发送 GET 请求
来源：https://rb.zhonguo6118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://le.zhonguo1118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://fd.zhonguo5118.cn

JS:   await fetch(url)
来源：https://kt.zhonguo1118.cn

TS:   await fetch(url)
来源：https://va.zhonguo8118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://tt.zhonguo2118.cn

Go:   resp, err := http.Get(url)
来源：https://xr.zhonguo2118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://lj.zhonguo6118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://ze.zhonguo8118.cn

[L02] 发送 POST JSON
来源：https://lb.zhonguo1118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://vu.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://xa.zhonguo5118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://sf.zhonguo5118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://bo.zhonguo7118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://sc.zhonguo1118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://ce.zhonguo5118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://bv.zhonguo8118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://nd.zhonguo8118.cn

[L03] 设置自定义请求头
来源：https://fn.zhonguo2118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://ma.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://vc.zhonguo5118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://fy.zhonguo8118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ym.zhonguo6118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://bm.zhonguo2118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://xu.zhonguo6118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://pt.zhonguo5118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://uy.zhonguo1118.cn

[L04] 设置超时
来源：https://gt.zhonguo6118.cn

Py:   requests.get(url, timeout=5)
来源：https://ti.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://ms.zhonguo3118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://sl.zhonguo5118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://sr.zhonguo6118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://dw.zhonguo3118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://fj.zhonguo4118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://wx.zhonguo1118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://nb.zhonguo1118.cn

[L05] 上传文件（multipart）
来源：https://jl.zhonguo4118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://ez.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://re.zhonguo1118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://bw.zhonguo1118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://av.zhonguo1118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://sc.zhonguo1118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://du.zhonguo3118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://nd.zhonguo2118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://zr.zhonguo7118.cn

[L06] 解析响应为 JSON
来源：https://yp.zhonguo3118.cn

Py:   resp.json()
来源：https://nb.zhonguo5118.cn

PHP:  json_decode($body, true);
来源：https://qg.zhonguo4118.cn

JS:   await resp.json()
来源：https://ks.zhonguo1118.cn

TS:   await resp.json()
来源：https://kv.zhonguo2118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://wk.zhonguo5118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://jk.zhonguo1118.cn

Ruby: JSON.parse(resp.body)
来源：https://ip.zhonguo4118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://la.zhonguo8118.cn

[L07] 处理 HTTP 状态码
来源：https://ki.zhonguo5118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://mu.zhonguo2118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://tu.zhonguo5118.cn

JS:   resp.ok;  resp.status
来源：https://dp.zhonguo8118.cn

TS:   resp.ok;  resp.status
来源：https://jf.zhonguo3118.cn

Java: resp.statusCode()
来源：https://kl.zhonguo2118.cn

Go:   resp.StatusCode
来源：https://wv.zhonguo5118.cn

Ruby: resp.code.to_i
来源：https://qe.zhonguo5118.cn

C#:   (int)resp.StatusCode
来源：https://yb.zhonguo1118.cn

[L08] 并发请求多个地址
来源：https://hh.zhonguo4118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://wz.zhonguo4118.cn

PHP:  curl_multi_init() 系列
来源：https://wg.zhonguo4118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ho.zhonguo1118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://yn.zhonguo6118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://vp.zhonguo7118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://qx.zhonguo5118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://ki.zhonguo2118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://ki.zhonguo3118.cn

================================================================================
来源：https://ab.zhonguo5118.cn

M. 命令行 / 进程 / 环境
来源：https://zz.zhonguo2118.cn

================================================================================
来源：https://be.zhonguo1118.cn

[M01] 读取命令行参数
来源：https://ih.zhonguo8118.cn

Py:   sys.argv[1:]
来源：https://hg.zhonguo4118.cn

PHP:  $argv;  $argc;
来源：https://ud.zhonguo7118.cn

JS:   process.argv.slice(2)
来源：https://ub.zhonguo7118.cn

TS:   process.argv.slice(2)
来源：https://mv.zhonguo4118.cn

Java: args 数组（main 方法参数）
来源：https://pj.zhonguo7118.cn

Go:   os.Args[1:]
来源：https://ou.zhonguo7118.cn

Ruby: ARGV
来源：https://rn.zhonguo5118.cn

C#:   args 数组（Main 方法参数）
来源：https://cp.zhonguo4118.cn

[M02] 读取环境变量
来源：https://az.zhonguo7118.cn

Py:   os.environ.get("HOME")
来源：https://wh.zhonguo6118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://ix.zhonguo5118.cn

JS:   process.env.HOME
来源：https://ez.zhonguo5118.cn

TS:   process.env.HOME
来源：https://qq.zhonguo7118.cn

Java: System.getenv("HOME")
来源：https://hs.zhonguo1118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://uh.zhonguo1118.cn

Ruby: ENV["HOME"]
来源：https://mj.zhonguo3118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://rt.zhonguo2118.cn

[M03] 执行外部命令
来源：https://ar.zhonguo5118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://va.zhonguo6118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://cy.zhonguo6118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://lb.zhonguo7118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://sm.zhonguo2118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://cy.zhonguo2118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://tc.zhonguo4118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://ge.zhonguo8118.cn

C#:   Process.Start("ls", "-l");
来源：https://or.zhonguo5118.cn

[M04] 获取当前工作目录
来源：https://pa.zhonguo4118.cn

Py:   os.getcwd()
来源：https://pj.zhonguo4118.cn

PHP:  getcwd();
来源：https://ak.zhonguo3118.cn

JS:   process.cwd()
来源：https://sl.zhonguo4118.cn

TS:   process.cwd()
来源：https://fy.zhonguo4118.cn

Java: Path.of("").toAbsolutePath()
来源：https://oi.zhonguo6118.cn

Go:   os.Getwd()
来源：https://bi.zhonguo3118.cn

Ruby: Dir.pwd
来源：https://zu.zhonguo3118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://mj.zhonguo7118.cn

[M05] 设置退出码
来源：https://dy.zhonguo5118.cn

Py:   sys.exit(1)
来源：https://lv.zhonguo8118.cn

PHP:  exit(1);
来源：https://gx.zhonguo6118.cn

JS:   process.exit(1)
来源：https://cz.zhonguo8118.cn

TS:   process.exit(1)
来源：https://bv.zhonguo7118.cn

Java: System.exit(1)
来源：https://lb.zhonguo8118.cn

Go:   os.Exit(1)
来源：https://zg.zhonguo8118.cn

Ruby: exit 1
来源：https://og.zhonguo6118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://hg.zhonguo4118.cn

[M06] 向标准错误输出
来源：https://it.zhonguo4118.cn

Py:   print("err", file=sys.stderr)
来源：https://iv.zhonguo7118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://sf.zhonguo8118.cn

JS:   console.error("err")
来源：https://cf.zhonguo4118.cn

TS:   console.error("err")
来源：https://jw.zhonguo6118.cn

Java: System.err.println("err")
来源：https://xb.zhonguo1118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://ai.zhonguo5118.cn

Ruby: warn "err"
来源：https://wr.zhonguo1118.cn

C#:   Console.Error.WriteLine("err")
来源：https://eb.zhonguo4118.cn

[M07] 判断是否为主入口
来源：https://ir.zhonguo2118.cn

Py:   if __name__ == "__main__":
来源：https://mw.zhonguo7118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://wl.zhonguo6118.cn

JS:   require.main === module
来源：https://ed.zhonguo1118.cn

TS:   require.main === module
来源：https://uy.zhonguo6118.cn

Java: public static void main(String[] args)
来源：https://cm.zhonguo8118.cn

Go:   func main()
来源：https://dg.zhonguo3118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://by.zhonguo8118.cn

C#:   static void Main(string[] args)
来源：https://sj.zhonguo2118.cn

[M08] 获取系统与运行时信息
来源：https://gd.zhonguo1118.cn

Py:   platform.system();  platform.python_version()
来源：https://gh.zhonguo2118.cn

PHP:  PHP_OS;  phpversion();
来源：https://ev.zhonguo4118.cn

JS:   process.platform;  process.version
来源：https://xm.zhonguo4118.cn

TS:   process.platform;  process.version
来源：https://xu.zhonguo8118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://rq.zhonguo1118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://cg.zhonguo1118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://he.zhonguo5118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://nr.zhonguo1118.cn

================================================================================
来源：https://mm.zhonguo1118.cn

N. 数据结构与算法
来源：https://pu.zhonguo8118.cn

================================================================================
来源：https://tp.zhonguo8118.cn

[N01] 二分查找（有序数组）
来源：https://ia.zhonguo7118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://gj.zhonguo2118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://fy.zhonguo5118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://xm.zhonguo7118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://rn.zhonguo4118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://vg.zhonguo6118.cn

Go:   sort.SearchInts(arr, x)
来源：https://hl.zhonguo3118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://lo.zhonguo6118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://cn.zhonguo6118.cn

[N02] 排序（工程实践用内置实现）
来源：https://zf.zhonguo1118.cn

Py:   sorted(arr);  arr.sort()
来源：https://do.zhonguo5118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://ue.zhonguo8118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://im.zhonguo4118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://ci.zhonguo6118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://vg.zhonguo8118.cn

Go:   slices.Sort(arr)
来源：https://ar.zhonguo5118.cn

Ruby: arr.sort
来源：https://yy.zhonguo5118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://oa.zhonguo5118.cn

[N03] 快速排序（分治示例）
来源：https://bx.zhonguo5118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://ge.zhonguo1118.cn

PHP:  // 递归实现，或用 usort
来源：https://pi.zhonguo6118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://xf.zhonguo7118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://ii.zhonguo2118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://eh.zhonguo5118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://sd.zhonguo3118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://hl.zhonguo8118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://lw.zhonguo6118.cn

[N04] 斐波那契数列
来源：https://ds.zhonguo4118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://fc.zhonguo7118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://hz.zhonguo6118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://bh.zhonguo7118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://uk.zhonguo3118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://ih.zhonguo3118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://lm.zhonguo1118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://mo.zhonguo8118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://qp.zhonguo1118.cn

[N05] 最大公约数
来源：https://oy.zhonguo6118.cn

Py:   math.gcd(a, b)
来源：https://ze.zhonguo6118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://da.zhonguo6118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://gn.zhonguo4118.cn


<!-- 参考信息 -->