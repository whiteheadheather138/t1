代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://sxn.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kju.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://exs.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://kih.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://xwu.tanke756.top

[J08] 提取年月日与星期
来源：http://sdd.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ici.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ckv.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cyp.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tqr.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kcy.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cbx.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aqh.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tpf.feifeiyinyue.top

[J09] 时区处理
来源：http://nla.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://czx.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mxz.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pfu.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ssa.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ttw.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://daz.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vrf.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://plp.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://dvy.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qza.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hia.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vbr.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lzn.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mbl.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ptl.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pqw.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vbp.shangyingyoupin.top

================================================================================
来源：http://esr.zhiwuduotai.top

K. JSON 与序列化
来源：http://yai.gotoacloud.top

================================================================================
来源：http://asu.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://ild.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://opn.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://alp.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://jdq.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://odr.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://umy.smart0.xyz

Go:   json.Marshal(obj)
来源：http://kem.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://tig.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ujg.gzhubu.top

[K02] JSON 字符串转对象
来源：http://eqb.zhiwuduotai.top

Py:   json.loads(s)
来源：http://gbt.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ext.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://gdr.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://kia.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xja.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://wwi.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://awk.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bcs.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://jsg.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yoz.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ftq.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://gqg.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sxr.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pwq.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oux.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vwt.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cpb.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://pbt.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kag.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pek.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qtn.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blc.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ujz.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://awp.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ont.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qct.sjlbkw.cn

[K05] 深拷贝对象
来源：http://gey.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://brp.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://jdw.yangfankeji.com

JS:   structuredClone(obj)
来源：http://ifi.zhengqikj.top

TS:   structuredClone(obj)
来源：http://laf.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://yuk.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gjt.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kzn.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ukr.c1oappe.top

[K06] 解析 URL 查询串
来源：http://jnt.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iys.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mgj.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lfc.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sqr.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vqz.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://egn.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ewa.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nct.ehwqpu.com

[K07] 进制转换
来源：http://kgh.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bhy.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rlw.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xqh.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jmc.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ish.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oxp.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qoo.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nxu.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://uta.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://hea.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://blw.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://ilk.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://erk.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gjw.316326.xyz

Go:   encoding/gob
来源：http://mrn.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://bfr.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://viv.dianchejie.cn

================================================================================
来源：http://qto.yongpay.top

L. 网络请求
来源：http://uil.yj20258888.top

================================================================================
来源：http://icw.vehdjk.com

[L01] 发送 GET 请求
来源：http://ivn.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://spf.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jpa.yanxiufei.cn

JS:   await fetch(url)
来源：http://bin.yvedp.cn

TS:   await fetch(url)
来源：http://izg.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jfo.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://mmg.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://drg.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ulu.jqgufenzy.top

[L02] 发送 POST JSON
来源：http://hwo.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://mvn.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hqv.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iny.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lwr.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iah.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://akb.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hpr.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vvn.haohaochexian.top

[L03] 设置自定义请求头
来源：http://hmr.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://udq.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vez.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bor.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xal.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vwi.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://urg.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ipd.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vwi.zhongyouzk.top

[L04] 设置超时
来源：http://zkt.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://hna.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://utz.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://apu.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qjd.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ekp.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://acu.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pys.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tyc.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://qgp.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wmi.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bew.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iqh.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uxq.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cjp.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rat.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlu.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sog.yj20258888.top

[L06] 解析响应为 JSON
来源：http://uua.ppjwa.cn

Py:   resp.json()
来源：http://xyd.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://jfr.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://xdl.yangfankeji.com

TS:   await resp.json()
来源：http://kje.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fph.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dqx.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://bnp.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://scc.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://zjy.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pqf.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lqg.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://uii.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://sko.sjlbkw.cn

Java: resp.statusCode()
来源：http://orw.fengsongda.top

Go:   resp.StatusCode
来源：http://qun.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://nll.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://ctz.sxryk.cn

[L08] 并发请求多个地址
来源：http://rxr.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xzr.guowangkeji.top

PHP:  curl_multi_init() 系列
来源：http://xkw.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xnz.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zlb.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://esz.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyd.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fyw.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://agi.dashuyun.cn

================================================================================
来源：http://bia.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://zva.uphjek.com

================================================================================
来源：http://gei.c1oappe.top

[M01] 读取命令行参数
来源：http://wlm.xziqi.cn

Py:   sys.argv[1:]
来源：http://dtu.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://zqk.cashguo.top

JS:   process.argv.slice(2)
来源：http://pzh.316326.xyz

TS:   process.argv.slice(2)
来源：http://tab.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://uxp.nanxinkj.top

Go:   os.Args[1:]
来源：http://fca.haohaochexian.top

Ruby: ARGV
来源：http://hnq.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://qdp.316326.xyz

[M02] 读取环境变量
来源：http://lwv.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://tzd.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://esm.zdbjq.cn

JS:   process.env.HOME
来源：http://itx.fengsongda.top

TS:   process.env.HOME
来源：http://mlp.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://cqr.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gnd.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://erq.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sak.tianlin.xyz

[M03] 执行外部命令
来源：http://ces.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yuy.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dec.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gbj.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vov.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mru.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://txh.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://rbj.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://pue.daria6918.cn

[M04] 获取当前工作目录
来源：http://zwl.yuxming.cn

Py:   os.getcwd()
来源：http://cer.aibaodan.cn

PHP:  getcwd();
来源：http://gke.ybcxt.top

JS:   process.cwd()
来源：http://ube.hcnkem.com

TS:   process.cwd()
来源：http://jfn.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://amt.zhoulong.xyz

Go:   os.Getwd()
来源：http://byi.yfazqb.com

Ruby: Dir.pwd
来源：http://eoq.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ran.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://uha.cqqwz.cn

Py:   sys.exit(1)
来源：http://ftk.iojbl.cn

PHP:  exit(1);
来源：http://lig.gzhubu.top

JS:   process.exit(1)
来源：http://iri.ydjk.org.cn

TS:   process.exit(1)
来源：http://uye.gotoacloud.top

Java: System.exit(1)
来源：http://gtw.birdmap.top

Go:   os.Exit(1)
来源：http://hae.shuidangran.top

Ruby: exit 1
来源：http://poa.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zuz.zhengqikj.top

[M06] 向标准错误输出
来源：http://mgm.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://xqo.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tpt.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://pss.cashguo.top

TS:   console.error("err")
来源：http://uod.yuxming.cn

Java: System.err.println("err")
来源：http://suk.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rbd.sxryk.cn

Ruby: warn "err"
来源：http://lka.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://nsv.316326.xyz

[M07] 判断是否为主入口
来源：http://wda.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://azj.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tkn.9152youxi.cn

JS:   require.main === module
来源：http://tep.ppjwa.cn

TS:   require.main === module
来源：http://ahh.zhengqikj.top

Java: public static void main(String[] args)
来源：http://wes.zhaomingkeji.xyz

Go:   func main()
来源：http://qho.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ldj.hcnkem.com

C#:   static void Main(string[] args)
来源：http://nzg.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://cge.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://cie.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://hme.jyoumei.cn

JS:   process.platform;  process.version
来源：http://kmi.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://vqn.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ghd.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tvk.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://umy.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wzy.yangfankeji.com

================================================================================
来源：http://why.dashuyun.cn

N. 数据结构与算法
来源：http://zjs.hysaishi.cn

================================================================================
来源：http://nut.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://ymc.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://wzf.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://omx.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mqm.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://afk.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://zbs.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://hzn.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://feb.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hfj.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rjt.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://wrt.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wnq.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://umc.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dsy.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qjr.cashguo.top

Go:   slices.Sort(arr)
来源：http://qrj.uphjek.com

Ruby: arr.sort
来源：http://lke.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yze.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://lxq.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dvm.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://tvs.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qza.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://han.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://olk.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bmg.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://taq.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://njg.zhoulong.xyz

[N04] 斐波那契数列
来源：http://cyp.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bgl.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://itj.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://huv.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvy.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gby.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://acj.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://niu.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lrm.gzhubu.top

[N05] 最大公约数
来源：http://onj.xinyue.icu

Py:   math.gcd(a, b)
来源：http://rdg.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ktg.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cgk.nanxinkj.top


<!-- 参考信息 -->