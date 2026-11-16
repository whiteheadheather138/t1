代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://fbn.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://skp.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hao.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://bwf.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://tqz.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://owi.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eou.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kpt.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nlk.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eij.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uth.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xch.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yla.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zgv.nwbrower.top

[J09] 时区处理
来源：http://zpm.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ang.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ayz.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rti.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qvy.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://poz.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wht.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://smh.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vzw.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://yzy.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lbs.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://olb.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jca.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dmi.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egv.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xrh.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xth.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rfz.smart0.xyz

================================================================================
来源：http://yna.zycfv.cn

K. JSON 与序列化
来源：http://xiv.yvedp.cn

================================================================================
来源：http://sze.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://llr.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vmw.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://edv.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://qnq.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://har.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://goa.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://vat.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://ber.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xoz.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://yhu.hywenlv.cn

Py:   json.loads(s)
来源：http://ily.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sea.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://mil.zhixingplan.top

TS:   JSON.parse(s)
来源：http://wxc.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pod.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ajx.hnqzz.top

Ruby: JSON.parse(s)
来源：http://fux.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rry.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://guy.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vwz.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://huj.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://efo.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://gff.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oyl.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tya.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hpx.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xxh.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://xst.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cnj.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://paa.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tai.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aws.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vke.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://clz.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cmo.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ydl.ydzc1.top

[K05] 深拷贝对象
来源：http://hny.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://kpx.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://oym.nanxinkj.top

JS:   structuredClone(obj)
来源：http://oor.hcnkem.com

TS:   structuredClone(obj)
来源：http://qtb.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qlp.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uir.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tqy.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iqk.yanxiufei.cn

[K06] 解析 URL 查询串
来源：http://lxh.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qgl.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yon.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yah.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uga.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://izq.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kfz.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hvz.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vcy.zhongyouzk.top

[K07] 进制转换
来源：http://tep.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ulu.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dci.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mmq.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eii.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bgb.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cet.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kmp.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tit.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://phj.yuxming.cn

Py:   pickle.dumps(obj)
来源：http://kao.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://cxq.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://uyj.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://bmz.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qul.daria6918.cn

Go:   encoding/gob
来源：http://mrv.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://pgk.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://chy.pycfn.com

================================================================================
来源：http://dbg.zhijiandao.cn

L. 网络请求
来源：http://bnf.yfazqb.com

================================================================================
来源：http://mhs.hcnkem.com

[L01] 发送 GET 请求
来源：http://meu.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kbm.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mdp.xziqi.cn

JS:   await fetch(url)
来源：http://cvp.zycfv.cn

TS:   await fetch(url)
来源：http://mxl.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://een.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://ogk.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mnc.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kus.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://tnz.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://oqx.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mgt.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://prh.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jkh.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vmr.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hby.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://deh.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zlw.snrcjt.cn

[L03] 设置自定义请求头
来源：http://zhc.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://axm.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lag.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxo.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ram.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uwf.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ork.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fep.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lyj.chenzaomai.com

[L04] 设置超时
来源：http://jjw.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://zvh.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ana.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jya.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bqr.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pel.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dvo.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dgm.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gre.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://zlc.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vrg.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nor.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qij.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jbt.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jnz.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kil.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tnf.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hoj.sweek.top

[L06] 解析响应为 JSON
来源：http://gnh.9152youxi.cn

Py:   resp.json()
来源：http://pcv.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://kov.fengsongda.top

JS:   await resp.json()
来源：http://nkq.tarul.cn

TS:   await resp.json()
来源：http://uyz.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bou.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://upq.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://tuh.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yzu.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://unh.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pnx.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://drj.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://hpq.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://aki.chenlongwang.top

Java: resp.statusCode()
来源：http://jcz.fzhhl.top

Go:   resp.StatusCode
来源：http://gzx.iojbl.cn

Ruby: resp.code.to_i
来源：http://eao.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://dor.tanke756.top

[L08] 并发请求多个地址
来源：http://slr.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bpf.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://bbh.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ygj.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pzx.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lox.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cts.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wcf.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pbo.jlsjyb.cn

================================================================================
来源：http://ihi.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://mbn.yj202588.top

================================================================================
来源：http://jyr.havefunace.top

[M01] 读取命令行参数
来源：http://mrx.ivvv.top

Py:   sys.argv[1:]
来源：http://hej.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://xdl.ydjk.org.cn

JS:   process.argv.slice(2)
来源：http://yzt.fengsongda.top

TS:   process.argv.slice(2)
来源：http://iwv.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://fcv.xuanzx.com

Go:   os.Args[1:]
来源：http://ofs.tian-w.cn

Ruby: ARGV
来源：http://irj.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://yik.havefunace.top

[M02] 读取环境变量
来源：http://dgw.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://gbf.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rnb.yvedp.cn

JS:   process.env.HOME
来源：http://xkh.zhongyouzk.top

TS:   process.env.HOME
来源：http://qvf.daria6918.cn

Java: System.getenv("HOME")
来源：http://psw.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oji.hammf.cn

Ruby: ENV["HOME"]
来源：http://xbd.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lmq.zhongyouzk.top

[M03] 执行外部命令
来源：http://snp.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jrh.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dbm.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://esl.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://smi.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://geq.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qjo.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://vew.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://err.fktsv.cn

[M04] 获取当前工作目录
来源：http://kjx.iojbl.cn

Py:   os.getcwd()
来源：http://ftq.zhijiandao.cn

PHP:  getcwd();
来源：http://jye.jinqigfzy.top

JS:   process.cwd()
来源：http://wtl.hammf.cn

TS:   process.cwd()
来源：http://rjt.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://sew.zhixingplan.top

Go:   os.Getwd()
来源：http://tiu.tianlin.xyz

Ruby: Dir.pwd
来源：http://sto.hcnkem.com

C#:   Directory.GetCurrentDirectory()
来源：http://bvs.ybcxt.top

[M05] 设置退出码
来源：http://cac.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://myq.gaohongyu789.top

PHP:  exit(1);
来源：http://gbo.shuidangran.top

JS:   process.exit(1)
来源：http://scj.hammf.cn

TS:   process.exit(1)
来源：http://dzj.xuetiantiany.cn

Java: System.exit(1)
来源：http://dql.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://owr.andypj.xyz

Ruby: exit 1
来源：http://fgb.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vej.yj20258.top

[M06] 向标准错误输出
来源：http://uxv.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://dtc.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ozk.hywenlv.cn

JS:   console.error("err")
来源：http://lqu.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://mgs.9152youxi.cn

Java: System.err.println("err")
来源：http://xzj.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://meh.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://ejn.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://nqm.tian-w.cn

[M07] 判断是否为主入口
来源：http://dwx.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://qdr.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wmw.c1oappe.top

JS:   require.main === module
来源：http://lfu.daria6918.cn

TS:   require.main === module
来源：http://ear.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://icp.fktsv.cn

Go:   func main()
来源：http://hkf.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kah.yuxming.cn

C#:   static void Main(string[] args)
来源：http://mjo.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://wff.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://ybq.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://xqg.wangdashe.top

JS:   process.platform;  process.version
来源：http://rfv.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://nbi.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://itz.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ebs.gzhubu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cbl.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oqj.zdqjudy.top

================================================================================
来源：http://bla.chenlongwang.top

N. 数据结构与算法
来源：http://qhg.ydjk.org.cn

================================================================================
来源：http://uid.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://gir.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yev.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fki.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://prv.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xji.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://bay.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://sio.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://miu.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://hhp.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://ruo.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://jke.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://epw.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://krv.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zxh.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://npe.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://ceb.feifeiyinyue.top

Ruby: arr.sort
来源：http://fkz.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sss.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://esr.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hnp.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://gre.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://crv.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dlq.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nrz.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xrf.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ktk.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tvv.fktsv.cn

[N04] 斐波那契数列
来源：http://xtq.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dmd.jinyuanbaomall.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fso.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jmy.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nuj.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://swt.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ljb.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qhk.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gph.ctjpmb.com

[N05] 最大公约数
来源：http://ary.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://gpt.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ehu.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zck.fanxiaobao.xyz


<!-- 参考信息 -->