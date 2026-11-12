代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://drg.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://khd.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zdt.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ahb.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xkk.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://npj.shzxlz.cn

[J09] 时区处理
来源：http://nxy.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qeq.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://noc.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vkm.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qjd.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nbt.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cck.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ygp.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uhz.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://pff.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wyl.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iqf.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://spe.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lhe.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bny.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zfe.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pri.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vdg.jqgfzy.top

================================================================================
来源：http://pcp.yanxiufei.cn

K. JSON 与序列化
来源：http://cgw.bbcook.cn

================================================================================
来源：http://dsu.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://yun.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kwb.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://enj.yonumen.top

JS:   JSON.stringify(obj)
来源：http://gbz.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://jfl.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gff.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://qij.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jye.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://knx.fengsongda.top

[K02] JSON 字符串转对象
来源：http://obe.sysykeji.top

Py:   json.loads(s)
来源：http://gbn.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://atm.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://wni.yuxming.cn

TS:   JSON.parse(s)
来源：http://hbl.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ael.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://mqi.tian-w.cn

Ruby: JSON.parse(s)
来源：http://hga.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hqb.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://bzx.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vem.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nsm.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://odd.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nzq.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uaw.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wed.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://ktp.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nvp.havefunace.top

[K04] 读取 JSON 文件
来源：http://xcf.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xay.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gov.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umd.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hie.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pwx.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nzv.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pgr.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dli.hcnkem.com

[K05] 深拷贝对象
来源：http://xnw.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://awg.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://mzr.cqqwz.cn

JS:   structuredClone(obj)
来源：http://oor.yvedp.cn

TS:   structuredClone(obj)
来源：http://akm.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qwi.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jvl.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qna.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://rmj.xylfe.cn

[K06] 解析 URL 查询串
来源：http://ibc.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wfg.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://atu.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rgr.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwa.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vlj.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lsl.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://faw.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ubh.yuxming.cn

[K07] 进制转换
来源：http://cyt.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jah.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vye.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yim.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xox.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eni.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://edb.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zvz.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rlk.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://rqq.sweek.top

Py:   pickle.dumps(obj)
来源：http://ktc.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qpe.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ahq.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://bww.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ulz.daxiang520.top

Go:   encoding/gob
来源：http://qoh.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://iku.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rhm.aizwys.cn

================================================================================
来源：http://djw.hysaishi.cn

L. 网络请求
来源：http://nyx.guowangkeji.top

================================================================================
来源：http://zro.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://zgw.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xei.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kaa.svipenyu.cn

JS:   await fetch(url)
来源：http://beh.daxiang520.top

TS:   await fetch(url)
来源：http://vmp.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wom.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://qtp.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zvv.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qui.havefunace.top

[L02] 发送 POST JSON
来源：http://fba.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uxx.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lqu.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xbp.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jog.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jdw.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iob.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ito.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bll.hesvh.cn

[L03] 设置自定义请求头
来源：http://mdl.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zdo.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mkd.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://snq.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ikd.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oww.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iff.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pkh.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vlx.xylfe.cn

[L04] 设置超时
来源：http://tmx.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://wek.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kdf.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvj.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zpa.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bep.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dxk.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://azj.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rnp.fehbvm.com

[L05] 上传文件（multipart）
来源：http://pnl.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://orm.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ryf.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yup.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ate.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cyp.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cqn.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vao.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kkk.mhx1999.top

[L06] 解析响应为 JSON
来源：http://tmt.shangyingyoupin.top

Py:   resp.json()
来源：http://lxy.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://ojg.gaohongyu789.top

JS:   await resp.json()
来源：http://spi.svipenyu.cn

TS:   await resp.json()
来源：http://dyr.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nwa.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vtk.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://xhj.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://enu.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://gzv.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aff.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ivw.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://lup.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://cst.yj20258.top

Java: resp.statusCode()
来源：http://wgk.yuanzhike.top

Go:   resp.StatusCode
来源：http://whc.xuanzx.com

Ruby: resp.code.to_i
来源：http://jzy.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://wol.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://zxf.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tyr.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://wwd.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sjd.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://edg.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wxd.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yzc.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dxl.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://enc.gaohongyu789.top

================================================================================
来源：http://oqx.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://tds.xingfuxueyuan.xyz

================================================================================
来源：http://uav.52xcode.cn

[M01] 读取命令行参数
来源：http://nfp.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://bju.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://uoh.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://nhi.52xcode.cn

TS:   process.argv.slice(2)
来源：http://pwa.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://lqc.yangfankeji.com

Go:   os.Args[1:]
来源：http://aqt.epnwcf.com

Ruby: ARGV
来源：http://dpc.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://biv.zhixingplan.top

[M02] 读取环境变量
来源：http://mrw.sweek.top

Py:   os.environ.get("HOME")
来源：http://lnt.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nvi.gogol.net.cn

JS:   process.env.HOME
来源：http://prh.uphjek.com

TS:   process.env.HOME
来源：http://qba.zycfv.cn

Java: System.getenv("HOME")
来源：http://hnt.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vcq.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://qks.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yqs.zdbjq.cn

[M03] 执行外部命令
来源：http://gud.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yqx.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vah.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://niz.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vwb.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cgb.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yeb.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wwe.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://rvt.yuxming.cn

[M04] 获取当前工作目录
来源：http://gvh.chenlongwang.top

Py:   os.getcwd()
来源：http://vtf.cucudq.cn

PHP:  getcwd();
来源：http://jku.zhongyouzk.top

JS:   process.cwd()
来源：http://qvk.hnxiangtu.top

TS:   process.cwd()
来源：http://jdj.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://fiz.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://goe.cucudq.cn

Ruby: Dir.pwd
来源：http://udf.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://hmz.hcnkem.com

[M05] 设置退出码
来源：http://qdk.yuanzhike.top

Py:   sys.exit(1)
来源：http://jgy.gotoacloud.top

PHP:  exit(1);
来源：http://qpt.nanxuanxn.top

JS:   process.exit(1)
来源：http://hqe.yangfankeji.com

TS:   process.exit(1)
来源：http://qah.hywenlv.cn

Java: System.exit(1)
来源：http://awp.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://aqf.yuxming.cn

Ruby: exit 1
来源：http://ckz.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fid.jqgufenzy.top

[M06] 向标准错误输出
来源：http://udo.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://ldr.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uvd.jyoumei.cn

JS:   console.error("err")
来源：http://pgf.bjfxy.top

TS:   console.error("err")
来源：http://brs.chenlongwang.top

Java: System.err.println("err")
来源：http://mdu.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jhk.xylfe.cn

Ruby: warn "err"
来源：http://sgz.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://biz.aizwys.cn

[M07] 判断是否为主入口
来源：http://uli.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://exb.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vbn.jqgfzy.top

JS:   require.main === module
来源：http://iiy.fengsongda.top

TS:   require.main === module
来源：http://tir.ivvv.top

Java: public static void main(String[] args)
来源：http://kmo.pengpengdd.cyou

Go:   func main()
来源：http://udx.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mym.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://lof.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://ddt.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://zij.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://reh.shzxlz.cn

JS:   process.platform;  process.version
来源：http://prr.gotoacloud.top

TS:   process.platform;  process.version
来源：http://dns.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jtq.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://cyy.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bvg.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yfx.gaohongyu789.top

================================================================================
来源：http://xqx.yangfankeji.com

N. 数据结构与算法
来源：http://pfk.cqqwz.cn

================================================================================
来源：http://ari.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://iwt.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://gnk.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://grl.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ujh.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rde.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://xne.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://tpl.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kyl.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wqg.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://qca.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://iql.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ucj.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://swr.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hyf.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://biy.smart0.xyz

Go:   slices.Sort(arr)
来源：http://qxn.gzhubu.top

Ruby: arr.sort
来源：http://uoj.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kxc.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://qgx.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gln.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://psx.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://exj.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsa.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wbd.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mhi.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wbx.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://esy.hywenlv.cn

[N04] 斐波那契数列
来源：http://cny.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gkz.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vfx.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mxu.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cnb.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wfz.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oar.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jqx.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cki.hywenlv.cn

[N05] 最大公约数
来源：http://bbd.bbcook.cn

Py:   math.gcd(a, b)
来源：http://vuc.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zsf.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://neq.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xes.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bqk.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://koq.yvedp.cn

Ruby: a.gcd(b)
来源：http://jrq.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nci.ehwqpu.com

[N06] 判断回文字符串
来源：http://mke.cqqwz.cn

Py:   s == s[::-1]
来源：http://keo.fengsongda.top

PHP:  $s === strrev($s);
来源：http://pvn.pycfn.com


<!-- 参考信息 -->