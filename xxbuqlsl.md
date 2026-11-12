代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://kla.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jxr.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cbw.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://aea.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://fds.smart0.xyz

[J08] 提取年月日与星期
来源：http://ogp.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pcd.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jtm.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ndd.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nwx.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nfd.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sll.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tcg.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blf.yangfankeji.com

[J09] 时区处理
来源：http://ark.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rmi.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ueb.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://noi.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rkn.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fqe.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ilz.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lbh.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://exx.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://sns.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gtv.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dkf.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vao.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gcm.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oxr.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wqp.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zeq.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://htn.fzhhl.top

================================================================================
来源：http://fju.pycfn.com

K. JSON 与序列化
来源：http://nyw.birdmap.top

================================================================================
来源：http://cgx.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://nws.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://skp.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://afz.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://eqn.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://fwx.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qps.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://xnk.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://xmu.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://myi.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://hzj.chenjidiqi.icu

Py:   json.loads(s)
来源：http://dkm.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bxu.316326.xyz

JS:   JSON.parse(s)
来源：http://xro.nwbrower.top

TS:   JSON.parse(s)
来源：http://wwx.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sds.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://crd.epnwcf.com

Ruby: JSON.parse(s)
来源：http://wbh.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wli.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://unm.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fja.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pqu.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zha.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wdh.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zkj.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uyc.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://btt.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://otz.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://nkm.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zsa.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://joo.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tcu.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lqw.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yra.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://drz.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bms.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://isr.nwbrower.top

[K05] 深拷贝对象
来源：http://lwt.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://ujw.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://frl.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://dgv.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://bli.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gdo.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qjn.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qpg.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kec.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://tjv.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oky.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fqp.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ahk.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fyg.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://arw.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ldp.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://caa.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ius.zhijiandao.cn

[K07] 进制转换
来源：http://gek.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://trc.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xob.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://swt.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://chb.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wqh.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qjz.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vzd.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wbt.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://zpc.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://kmu.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://svo.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://fds.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://dhy.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ibz.hongshengwenyu.top

Go:   encoding/gob
来源：http://jie.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://fix.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iac.cucudq.cn

================================================================================
来源：http://gph.shzxlz.cn

L. 网络请求
来源：http://frg.tianlin.xyz

================================================================================
来源：http://mdk.aibaodan.cn

[L01] 发送 GET 请求
来源：http://fag.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zbl.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gut.jianghu66.top

JS:   await fetch(url)
来源：http://ojo.ydzc1.top

TS:   await fetch(url)
来源：http://bra.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ukl.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://mpl.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://llb.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qhm.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://jwm.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://rtr.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rdx.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgd.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nqw.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://afb.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://icf.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tzt.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ryb.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://vew.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qqg.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wwn.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqi.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bgm.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nhd.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iuk.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dfz.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jbi.daxiang520.top

[L04] 设置超时
来源：http://ppt.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://kfe.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rct.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://udq.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nmi.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cmx.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fwj.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ahr.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pvf.hesvh.cn

[L05] 上传文件（multipart）
来源：http://kbc.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cnp.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://teb.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://slf.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xtf.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://por.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wor.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yiz.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://agg.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://otm.jinqigufen.top

Py:   resp.json()
来源：http://qmg.xylfe.cn

PHP:  json_decode($body, true);
来源：http://cxk.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://opc.havefunace.top

TS:   await resp.json()
来源：http://usn.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cjg.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bra.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://euc.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://twf.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://mua.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pqr.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cjw.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://szd.tarul.cn

TS:   resp.ok;  resp.status
来源：http://njc.bbcook.cn

Java: resp.statusCode()
来源：http://tpg.jqgufenzy.top

Go:   resp.StatusCode
来源：http://hfx.hysaishi.cn

Ruby: resp.code.to_i
来源：http://mdi.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://hrk.yvedp.cn

[L08] 并发请求多个地址
来源：http://ejl.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iid.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://lhv.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uln.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sgs.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rzq.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ski.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yjx.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cwp.havefunace.top

================================================================================
来源：http://bgg.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://scd.daria6918.cn

================================================================================
来源：http://rzr.tanke756.top

[M01] 读取命令行参数
来源：http://odn.gzhubu.top

Py:   sys.argv[1:]
来源：http://eic.vehdjk.com

PHP:  $argv;  $argc;
来源：http://jxl.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://zyk.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://zqs.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://har.jinqigufen.top

Go:   os.Args[1:]
来源：http://hql.zhiwuduotai.top

Ruby: ARGV
来源：http://ywe.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://ibg.cucudq.cn

[M02] 读取环境变量
来源：http://bqb.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://vxp.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gmo.yvedp.cn

JS:   process.env.HOME
来源：http://oak.hesvh.cn

TS:   process.env.HOME
来源：http://tbb.gotoacloud.top

Java: System.getenv("HOME")
来源：http://wjj.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wqa.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://iiu.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vjo.xuanzx.com

[M03] 执行外部命令
来源：http://nuf.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iqt.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ggr.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zzh.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://imu.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ilw.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vdy.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fuf.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://gbk.xuetiantiany.cn

[M04] 获取当前工作目录
来源：http://amk.cheryme.top

Py:   os.getcwd()
来源：http://lga.zhiwuduotai.top

PHP:  getcwd();
来源：http://ccf.hesvh.cn

JS:   process.cwd()
来源：http://vfi.tianlin.xyz

TS:   process.cwd()
来源：http://zax.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://lzf.ydzc1.top

Go:   os.Getwd()
来源：http://wzb.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://bst.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yzc.sxryk.cn

[M05] 设置退出码
来源：http://hro.jinqigufen.top

Py:   sys.exit(1)
来源：http://idf.vehdjk.com

PHP:  exit(1);
来源：http://flq.jqgufenzy.top

JS:   process.exit(1)
来源：http://aoy.zdqjudy.top

TS:   process.exit(1)
来源：http://prg.zhoulong.xyz

Java: System.exit(1)
来源：http://sqw.9152youxi.cn

Go:   os.Exit(1)
来源：http://ddg.cheryme.top

Ruby: exit 1
来源：http://ijj.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://thx.tanke756.top

[M06] 向标准错误输出
来源：http://msl.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://loz.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vhl.cqqwz.cn

JS:   console.error("err")
来源：http://azl.fanxiaobao.xyz

TS:   console.error("err")
来源：http://urg.gotoacloud.top

Java: System.err.println("err")
来源：http://ttj.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gge.xylfe.cn

Ruby: warn "err"
来源：http://qix.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://iki.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://qqu.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://efv.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oet.zhiwuduotai.top

JS:   require.main === module
来源：http://vbs.quarkkingdee.top

TS:   require.main === module
来源：http://jjz.bbcook.cn

Java: public static void main(String[] args)
来源：http://uzw.xuanzx.com

Go:   func main()
来源：http://bpa.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fhs.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://gyy.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://xdz.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://tdi.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://mbp.sxryk.cn

JS:   process.platform;  process.version
来源：http://qmn.iojbl.cn

TS:   process.platform;  process.version
来源：http://bvq.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tfv.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://myr.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vvl.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ygd.tian-w.cn

================================================================================
来源：http://bjj.9152youxi.cn

N. 数据结构与算法
来源：http://ton.nwbrower.top

================================================================================
来源：http://yuc.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://qog.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fbl.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lbx.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aro.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpe.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://fin.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://moq.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://lof.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lhk.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://bns.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xrm.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vec.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vhh.vqdsnc.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jej.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pwk.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://cei.zhixingplan.top

Ruby: arr.sort
来源：http://ggo.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bow.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://pck.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wkz.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://zii.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvx.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fjx.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oew.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zvj.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://trv.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://kpb.fzhhl.top

[N04] 斐波那契数列
来源：http://lxa.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nrk.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kdg.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pil.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://glh.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ggl.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wee.ctjpmb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewu.tianlin.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lzr.shuidangran.top

[N05] 最大公约数
来源：http://azx.zycfv.cn

Py:   math.gcd(a, b)
来源：http://jxz.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ffi.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gxr.yvedp.cn


<!-- 参考信息 -->