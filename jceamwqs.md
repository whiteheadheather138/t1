代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://nuf.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://scy.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gzx.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lrn.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://lvy.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://gbd.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uvd.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cfu.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mav.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rxx.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bfx.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dbo.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fyk.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eei.hammf.cn

[J09] 时区处理
来源：http://mzj.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ayx.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cpb.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogm.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uvq.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hxc.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ahr.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rqh.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://flf.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://dzo.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fhw.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ket.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sol.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dqf.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oax.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cxh.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ahr.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ljo.hesvh.cn

================================================================================
来源：http://wib.andypj.xyz

K. JSON 与序列化
来源：http://fjo.yangfankeji.com

================================================================================
来源：http://ojt.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://lrf.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nyd.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gge.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://eia.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://jen.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hdx.cucudq.cn

Go:   json.Marshal(obj)
来源：http://gil.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pvp.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://inb.meibo888.top

[K02] JSON 字符串转对象
来源：http://tli.nanxuanxn.top

Py:   json.loads(s)
来源：http://jnw.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xdx.tanke756.top

JS:   JSON.parse(s)
来源：http://iev.gzhubu.top

TS:   JSON.parse(s)
来源：http://bmw.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://phs.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://iwg.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://rgn.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qla.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://rpi.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rsh.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://szx.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oga.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zmv.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mcl.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tlu.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://cjd.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rou.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://qtg.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fyt.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nnp.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwp.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rae.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kyx.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dkv.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dbq.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hhl.meibo888.top

[K05] 深拷贝对象
来源：http://mdq.sweek.top

Py:   copy.deepcopy(obj)
来源：http://jbv.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://uyy.epnwcf.com

JS:   structuredClone(obj)
来源：http://yks.yuxming.cn

TS:   structuredClone(obj)
来源：http://kdq.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xqu.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://epi.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eiq.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ebs.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://qwa.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://haz.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nbg.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ubs.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qvo.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yuw.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dbt.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tsd.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rlf.xziqi.cn

[K07] 进制转换
来源：http://pzn.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mfx.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lip.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ffk.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ghu.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vts.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rey.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gue.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bkh.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://pwt.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://mtp.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qtz.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://tox.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://iws.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ide.wangdashe.top

Go:   encoding/gob
来源：http://gxy.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://akv.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hev.quarkkingdee.top

================================================================================
来源：http://hxo.wangshuangyany.cn

L. 网络请求
来源：http://cme.jiagoushi.top

================================================================================
来源：http://qrl.jinqigufen.top

[L01] 发送 GET 请求
来源：http://vvd.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qjd.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://izz.cdnleiting.top

JS:   await fetch(url)
来源：http://hmt.quarkkingdee.top

TS:   await fetch(url)
来源：http://hme.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://byt.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://hxs.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vdk.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zch.xuanzx.com

[L02] 发送 POST JSON
来源：http://jng.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kdx.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://swl.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyw.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rpe.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rmv.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nze.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ztt.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fad.yfazqb.com

[L03] 设置自定义请求头
来源：http://tft.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bnw.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vso.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jay.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynz.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lkv.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iza.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bcm.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vhf.9152youxi.cn

[L04] 设置超时
来源：http://dbn.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://kgg.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mmm.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eir.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bkh.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://crm.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://isl.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yfu.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lvv.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://sog.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://acp.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mec.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ajf.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qsc.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uul.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ily.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xxh.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gvb.guannengcc.top

[L06] 解析响应为 JSON
来源：http://efd.bjfxy.top

Py:   resp.json()
来源：http://fsc.pycfn.com

PHP:  json_decode($body, true);
来源：http://snn.ydjk.org.cn

JS:   await resp.json()
来源：http://dzd.xuetiantiany.cn

TS:   await resp.json()
来源：http://lqv.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://chh.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://umx.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://cme.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wfm.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://wsw.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qmb.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://awi.ivvv.top

JS:   resp.ok;  resp.status
来源：http://gee.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://aax.zhijiandao.cn

Java: resp.statusCode()
来源：http://qug.jlsjyb.cn

Go:   resp.StatusCode
来源：http://rui.fzhhl.top

Ruby: resp.code.to_i
来源：http://iuo.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://pli.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://pti.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aup.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://glg.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpl.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mks.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rgf.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xkr.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yiq.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zpy.havefunace.top

================================================================================
来源：http://swr.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://nul.snrcjt.cn

================================================================================
来源：http://eji.cqqwz.cn

[M01] 读取命令行参数
来源：http://rzw.guannengcc.top

Py:   sys.argv[1:]
来源：http://euc.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://qew.vehdjk.com

JS:   process.argv.slice(2)
来源：http://qkw.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://tmr.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://jlh.zhongyouzk.top

Go:   os.Args[1:]
来源：http://rus.yfazqb.com

Ruby: ARGV
来源：http://igh.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://qnt.jyoumei.cn

[M02] 读取环境变量
来源：http://tkn.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://fqo.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://faq.zdbjq.cn

JS:   process.env.HOME
来源：http://lkk.yj20258888.top

TS:   process.env.HOME
来源：http://ekf.smart0.xyz

Java: System.getenv("HOME")
来源：http://haw.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tsh.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://cga.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fpz.0kj1m.cn

[M03] 执行外部命令
来源：http://tda.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lqw.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pqa.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ggf.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fgt.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://trg.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ahc.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://wup.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://vii.yongpay.top

[M04] 获取当前工作目录
来源：http://lkz.yuanzhike.top

Py:   os.getcwd()
来源：http://xgz.fktsv.cn

PHP:  getcwd();
来源：http://gfr.shangyingyoupin.top

JS:   process.cwd()
来源：http://chc.sxryk.cn

TS:   process.cwd()
来源：http://ulp.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://tma.bjfxy.top

Go:   os.Getwd()
来源：http://cmp.yueranfly.top

Ruby: Dir.pwd
来源：http://xhz.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://aur.yuxming.cn

[M05] 设置退出码
来源：http://xno.zhixingplan.top

Py:   sys.exit(1)
来源：http://msw.hammf.cn

PHP:  exit(1);
来源：http://pps.xziqi.cn

JS:   process.exit(1)
来源：http://kiv.pengpengdd.cyou

TS:   process.exit(1)
来源：http://xdt.nanxinkj.top

Java: System.exit(1)
来源：http://ldo.cucudq.cn

Go:   os.Exit(1)
来源：http://ycq.fanxiaobao.xyz

Ruby: exit 1
来源：http://nkq.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kvo.sysykeji.top

[M06] 向标准错误输出
来源：http://qvn.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://slb.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://byx.bjfxy.top

JS:   console.error("err")
来源：http://sfl.pengpengdd.cyou

TS:   console.error("err")
来源：http://iod.iojbl.cn

Java: System.err.println("err")
来源：http://yxz.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mqh.ybcxt.top

Ruby: warn "err"
来源：http://vwg.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://unq.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://axo.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://vyd.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ndp.tarul.cn

JS:   require.main === module
来源：http://nhf.zhixingplan.top

TS:   require.main === module
来源：http://pso.fzhhl.top

Java: public static void main(String[] args)
来源：http://ugf.zhongyouzk.top

Go:   func main()
来源：http://ljj.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://njr.aizwys.cn

C#:   static void Main(string[] args)
来源：http://tzd.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://qzj.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://mne.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://ixx.tianlin.xyz

JS:   process.platform;  process.version
来源：http://lzt.hysaishi.cn

TS:   process.platform;  process.version
来源：http://har.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://anl.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cdp.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://guy.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nid.hongshengwenyu.top

================================================================================
来源：http://czm.andypj.xyz

N. 数据结构与算法
来源：http://ikm.0kj1m.cn

================================================================================
来源：http://ora.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://dod.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://fdg.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://isd.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oxy.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urv.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://als.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://ggs.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://buj.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://joo.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://eap.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://iki.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ypn.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vyr.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://plj.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xpv.sysykeji.top

Go:   slices.Sort(arr)
来源：http://ztk.andypj.xyz

Ruby: arr.sort
来源：http://oyz.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ncu.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://ypw.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wan.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://cii.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rld.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nue.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aob.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zpj.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pvv.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://lar.yj202588.top

[N04] 斐波那契数列
来源：http://atj.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lwd.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vob.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wcr.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ccn.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dnc.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://txp.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sfa.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ujo.sweek.top

[N05] 最大公约数
来源：http://fqh.tian-w.cn

Py:   math.gcd(a, b)
来源：http://xox.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uyd.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rrm.zycfv.cn


<!-- 参考信息 -->