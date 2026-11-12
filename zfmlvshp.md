代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://bwk.sweek.top

[J08] 提取年月日与星期
来源：http://ysg.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bdm.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jli.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kdj.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ylu.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lcr.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cwy.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ooi.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://srz.shangyingyoupin.top

[J09] 时区处理
来源：http://ggf.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kww.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eml.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tvv.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://arm.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bnp.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uby.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kfo.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ieb.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://ipp.shanyushiyangtech.top

Py:   date.today();  date.today().replace(day=1)
来源：http://aoc.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jdg.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cps.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://plw.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qnj.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pka.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ghh.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pii.haohaochexian.top

================================================================================
来源：http://xbm.aibaodan.cn

K. JSON 与序列化
来源：http://pcn.hammf.cn

================================================================================
来源：http://lrr.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://awo.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dif.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gnw.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://noy.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://huh.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gwm.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://iak.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yip.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dwt.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://lnf.epnwcf.com

Py:   json.loads(s)
来源：http://zad.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fbk.shzxlz.cn

JS:   JSON.parse(s)
来源：http://tgh.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://hpy.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zxq.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://gby.fehbvm.com

Ruby: JSON.parse(s)
来源：http://whs.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eok.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://ltf.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vod.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nve.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qns.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fha.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nhl.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nxt.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kpw.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wzr.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://nno.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vxw.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bnv.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iyh.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wky.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hdq.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fyl.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://xwu.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kso.chenlongwang.top

[K05] 深拷贝对象
来源：http://hfp.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://dzm.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://oii.gotoacloud.top

JS:   structuredClone(obj)
来源：http://qwq.shuidangran.top

TS:   structuredClone(obj)
来源：http://sdn.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yjz.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gnn.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tbi.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qup.ivvv.top

[K06] 解析 URL 查询串
来源：http://eep.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pug.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jse.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xku.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://epa.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lnq.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sed.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rxi.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ben.hywenlv.cn

[K07] 进制转换
来源：http://rnl.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mse.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hyx.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ixo.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ddb.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eze.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://scg.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hmg.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rxc.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://qme.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://qaf.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tux.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://chm.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://kbj.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nwh.shzxlz.cn

Go:   encoding/gob
来源：http://hwn.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://ooc.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ygl.sufxvd.cn

================================================================================
来源：http://yed.pengpengdd.cyou

L. 网络请求
来源：http://lwo.cucudq.cn

================================================================================
来源：http://fmm.c1oappe.top

[L01] 发送 GET 请求
来源：http://yun.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rhi.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hsr.sjlbkw.cn

JS:   await fetch(url)
来源：http://wpa.hfpthk.cn

TS:   await fetch(url)
来源：http://uek.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fcw.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://ace.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://luj.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lce.shuidangran.top

[L02] 发送 POST JSON
来源：http://qzt.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wur.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bwm.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pns.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://imh.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rzh.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://stg.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lge.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iln.sxryk.cn

[L03] 设置自定义请求头
来源：http://fth.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://psb.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aqn.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cxl.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbf.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://npe.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dyr.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://huh.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fww.nanxinkj.top

[L04] 设置超时
来源：http://esc.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://aba.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dpq.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zac.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qcq.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://awk.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xrj.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cqv.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pje.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://oaa.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://krw.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://emp.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gzf.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uow.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eps.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tvr.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pnh.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://foo.yj20258.top

[L06] 解析响应为 JSON
来源：http://fuf.ydzc1.top

Py:   resp.json()
来源：http://uii.jinghuilouyu.cn

PHP:  json_decode($body, true);
来源：http://vra.pengpengdd.cyou

JS:   await resp.json()
来源：http://lht.fzhhl.top

TS:   await resp.json()
来源：http://pmu.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fcy.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vdw.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://zex.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qjj.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://prn.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ygc.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vhl.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://vzn.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://xjz.zhijiandao.cn

Java: resp.statusCode()
来源：http://xjv.iojbl.cn

Go:   resp.StatusCode
来源：http://mfq.snrcjt.cn

Ruby: resp.code.to_i
来源：http://ibz.meibo888.top

C#:   (int)resp.StatusCode
来源：http://qsq.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://kex.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dnd.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://asc.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zqn.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nzs.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bmt.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rff.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vwi.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cvc.fengsongda.top

================================================================================
来源：http://tgj.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://afs.daria6918.cn

================================================================================
来源：http://jjl.yuanzhike.top

[M01] 读取命令行参数
来源：http://hvh.sufxvd.cn

Py:   sys.argv[1:]
来源：http://vtw.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://ibi.daxiang520.top

JS:   process.argv.slice(2)
来源：http://agh.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://zvb.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://eao.guannengcc.top

Go:   os.Args[1:]
来源：http://rrp.0kj1m.cn

Ruby: ARGV
来源：http://qfl.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://bsd.cheryme.top

[M02] 读取环境变量
来源：http://nov.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://usp.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kdg.svipenyu.cn

JS:   process.env.HOME
来源：http://dif.316326.xyz

TS:   process.env.HOME
来源：http://ehw.hywenlv.cn

Java: System.getenv("HOME")
来源：http://rlw.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://knn.yueranfly.top

Ruby: ENV["HOME"]
来源：http://dkq.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wjo.yangfankeji.com

[M03] 执行外部命令
来源：http://wly.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gps.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vvi.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://pck.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tao.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pbw.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://irw.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hde.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://zla.cdnleiting.top

[M04] 获取当前工作目录
来源：http://dwr.yvedp.cn

Py:   os.getcwd()
来源：http://sac.hammf.cn

PHP:  getcwd();
来源：http://lmk.wangdashe.top

JS:   process.cwd()
来源：http://myq.nwbrower.top

TS:   process.cwd()
来源：http://nky.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://tbc.birdmap.top

Go:   os.Getwd()
来源：http://okd.shzxlz.cn

Ruby: Dir.pwd
来源：http://cpu.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://soh.shangyingyoupin.top

[M05] 设置退出码
来源：http://rqk.birdmap.top

Py:   sys.exit(1)
来源：http://sug.jinqigufen.top

PHP:  exit(1);
来源：http://csn.tian-w.cn

JS:   process.exit(1)
来源：http://cih.quarkkingdee.top

TS:   process.exit(1)
来源：http://zmh.hywenlv.cn

Java: System.exit(1)
来源：http://sng.0kj1m.cn

Go:   os.Exit(1)
来源：http://fth.yanxiufei.cn

Ruby: exit 1
来源：http://qzy.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zms.yvedp.cn

[M06] 向标准错误输出
来源：http://thi.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://oqr.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ody.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://mst.yfazqb.com

TS:   console.error("err")
来源：http://bnf.daria6918.cn

Java: System.err.println("err")
来源：http://ftx.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ovh.mhx1999.top

Ruby: warn "err"
来源：http://lhp.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://wje.havefunace.top

[M07] 判断是否为主入口
来源：http://epa.hammf.cn

Py:   if __name__ == "__main__":
来源：http://xpr.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hfh.hammf.cn

JS:   require.main === module
来源：http://hpd.nanxinkj.top

TS:   require.main === module
来源：http://ndx.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://itm.guannengcc.top

Go:   func main()
来源：http://muo.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://toi.yj202588.top

C#:   static void Main(string[] args)
来源：http://psh.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://lhc.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://wxv.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://ftd.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://xug.dianchejie.cn

TS:   process.platform;  process.version
来源：http://dgw.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oqq.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ttn.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qpr.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xvf.iojbl.cn

================================================================================
来源：http://uaq.uphjek.com

N. 数据结构与算法
来源：http://tpq.mhx1999.top

================================================================================
来源：http://hyl.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://req.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://bof.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://inp.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vwf.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qhx.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://xjt.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://dze.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://nxr.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://yqv.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://bvi.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://wcb.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iqb.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gqb.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iwb.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oup.pycfn.com

Go:   slices.Sort(arr)
来源：http://zvy.cheryme.top

Ruby: arr.sort
来源：http://hip.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lhc.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://tnt.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fcs.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://tcr.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dik.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xro.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://avq.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bva.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gaq.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ipd.zhoulong.xyz

[N04] 斐波那契数列
来源：http://llr.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dpu.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wpb.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oka.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://usv.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://swu.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lrc.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zrt.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tkh.cdnleiting.top

[N05] 最大公约数
来源：http://gbs.yj20258.top

Py:   math.gcd(a, b)
来源：http://ktb.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uiw.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kxo.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfj.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cbh.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://voa.nanxinkj.top

Ruby: a.gcd(b)
来源：http://loh.hongshengwenyu.top


<!-- 参考信息 -->