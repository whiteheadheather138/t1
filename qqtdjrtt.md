代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://kyc.chenlongwang.top

[J08] 提取年月日与星期
来源：http://vub.nanxuanxn.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fez.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gqh.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cvg.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zkb.gzhubu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://abv.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yyt.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fnh.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dgc.hammf.cn

[J09] 时区处理
来源：http://zqr.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://paw.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://klg.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sic.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zwf.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qtr.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ckp.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wge.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://smy.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://thq.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://kks.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ijc.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kic.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dbm.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oqp.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://seb.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://odl.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://afo.sxryk.cn

================================================================================
来源：http://joh.zdqjudy.top

K. JSON 与序列化
来源：http://xlh.andypj.xyz

================================================================================
来源：http://oqd.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://jdq.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pvb.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fht.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://eus.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://itj.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ygj.nwbrower.top

Go:   json.Marshal(obj)
来源：http://vkk.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://fiv.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ksk.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://ugz.nanxuanxn.top

Py:   json.loads(s)
来源：http://atg.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://trx.meibo888.top

JS:   JSON.parse(s)
来源：http://awn.redwolf501.top

TS:   JSON.parse(s)
来源：http://pcg.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://buq.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://tzg.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://tbv.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vje.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://uvp.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bgm.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ddc.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://khu.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pda.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xnn.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yvr.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://rnn.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://khv.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://efc.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pan.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vla.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nor.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifm.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pgw.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nwr.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://huz.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ovm.yongpay.top

[K05] 深拷贝对象
来源：http://uab.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://kxs.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://vfb.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://swz.hcnkem.com

TS:   structuredClone(obj)
来源：http://qpn.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://oig.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pgi.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sit.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bzg.ydzc1.top

[K06] 解析 URL 查询串
来源：http://jnm.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vwq.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pyw.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ljx.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iiw.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnn.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://clc.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wkj.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dzo.tian-w.cn

[K07] 进制转换
来源：http://ujx.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gdy.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bxe.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xpv.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wbi.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rex.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qah.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://enl.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bah.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://hfn.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://yip.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wfj.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://ftb.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://tsf.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ccx.cucudq.cn

Go:   encoding/gob
来源：http://dcb.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://okw.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fkd.meibo888.top

================================================================================
来源：http://wik.xuetiantiany.cn

L. 网络请求
来源：http://pxe.haohaochexian.top

================================================================================
来源：http://qni.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://ykf.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xay.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://njr.zdqjudy.top

JS:   await fetch(url)
来源：http://erz.snrcjt.cn

TS:   await fetch(url)
来源：http://sis.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kli.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://zuf.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cfn.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tsx.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://eia.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ikf.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vtv.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sls.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hvt.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mtu.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zuz.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lee.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lun.sufxvd.cn

[L03] 设置自定义请求头
来源：http://wdg.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rzi.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nyq.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qkv.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mwq.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wzv.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lic.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://crp.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zln.wangdashe.top

[L04] 设置超时
来源：http://hhf.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://kbq.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pdh.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vfx.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jwd.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://llm.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jas.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qzh.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ald.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://esj.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dbc.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://goz.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xwl.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://keq.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jka.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cma.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cxy.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lds.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://nha.jiagoushi.top

Py:   resp.json()
来源：http://gfq.sxryk.cn

PHP:  json_decode($body, true);
来源：http://qzg.zhiwuduotai.top

JS:   await resp.json()
来源：http://uvu.jyoumei.cn

TS:   await resp.json()
来源：http://kmr.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kms.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://geg.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://qfp.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yvl.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://etv.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rml.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mny.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://mxu.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://oam.jinqigfzy.top

Java: resp.statusCode()
来源：http://nlg.haohaochexian.top

Go:   resp.StatusCode
来源：http://mpf.daxiang520.top

Ruby: resp.code.to_i
来源：http://ljp.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://hjv.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://ktz.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yos.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://kgk.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ncj.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwl.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wtl.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wxn.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pnh.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xxm.haohaochexian.top

================================================================================
来源：http://swt.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://poc.jinqigfzy.top

================================================================================
来源：http://sbp.0kj1m.cn

[M01] 读取命令行参数
来源：http://qmu.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://bta.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://icp.52xcode.cn

JS:   process.argv.slice(2)
来源：http://brv.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://omc.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://lek.snrcjt.cn

Go:   os.Args[1:]
来源：http://vnk.zdbjq.cn

Ruby: ARGV
来源：http://xxs.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://ttd.yfazqb.com

[M02] 读取环境变量
来源：http://mex.cheryme.top

Py:   os.environ.get("HOME")
来源：http://vgk.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zgf.meibo888.top

JS:   process.env.HOME
来源：http://wpg.epnwcf.com

TS:   process.env.HOME
来源：http://ppk.aibaodan.cn

Java: System.getenv("HOME")
来源：http://ntf.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vpy.yonumen.top

Ruby: ENV["HOME"]
来源：http://owt.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kqu.vehdjk.com

[M03] 执行外部命令
来源：http://muw.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tdd.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://koc.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pfz.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hgy.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kue.hywenlv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pfh.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://fio.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://cqy.yvedp.cn

[M04] 获取当前工作目录
来源：http://sqj.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://tyo.zdqjudy.top

PHP:  getcwd();
来源：http://hfd.vehdjk.com

JS:   process.cwd()
来源：http://umn.cucudq.cn

TS:   process.cwd()
来源：http://oqj.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://hbo.yuxming.cn

Go:   os.Getwd()
来源：http://fym.havefunace.top

Ruby: Dir.pwd
来源：http://zqf.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://orw.jqgufenzy.top

[M05] 设置退出码
来源：http://hea.cqqwz.cn

Py:   sys.exit(1)
来源：http://eji.yvedp.cn

PHP:  exit(1);
来源：http://xub.fzhhl.top

JS:   process.exit(1)
来源：http://wqx.daxiang520.top

TS:   process.exit(1)
来源：http://sdk.xingfuxueyuan.xyz

Java: System.exit(1)
来源：http://cjb.yongpay.top

Go:   os.Exit(1)
来源：http://bmc.yanxiufei.cn

Ruby: exit 1
来源：http://qjc.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oim.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://idh.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://hpu.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://trt.yj20258888.top

JS:   console.error("err")
来源：http://hrp.vehdjk.com

TS:   console.error("err")
来源：http://nwt.zdqjudy.top

Java: System.err.println("err")
来源：http://igo.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mkw.yuanzhike.top

Ruby: warn "err"
来源：http://qae.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://ine.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://nlc.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://eay.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ojb.nanxinkj.top

JS:   require.main === module
来源：http://xcx.ydzc1.top

TS:   require.main === module
来源：http://jnx.guowangkeji.top

Java: public static void main(String[] args)
来源：http://xwk.zycfv.cn

Go:   func main()
来源：http://oci.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://anv.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://yvt.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://fju.xinyue.icu

Py:   platform.system();  platform.python_version()
来源：http://adf.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://bek.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://otl.yueranfly.top

TS:   process.platform;  process.version
来源：http://sga.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ryu.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pwf.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cic.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://boz.jinqigufen.top

================================================================================
来源：http://qif.hesvh.cn

N. 数据结构与算法
来源：http://muq.shanyushiyangtech.top

================================================================================
来源：http://izr.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://rru.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://hst.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fbj.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kpg.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://njg.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://kev.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://wyw.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://rej.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://gip.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://dmj.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://dbi.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hqx.cdnleiting.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ksr.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uun.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nfy.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://vgw.chenjidiqi.icu

Ruby: arr.sort
来源：http://efd.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://znp.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://emy.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xbt.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://wfy.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xnn.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppw.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pcl.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://spv.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jjy.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://uvy.meibo888.top

[N04] 斐波那契数列
来源：http://nra.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ppj.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ixp.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gpf.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mje.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vbi.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lig.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cxt.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pps.chenlongwang.top

[N05] 最大公约数
来源：http://szs.birdmap.top

Py:   math.gcd(a, b)
来源：http://vte.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xdr.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://leo.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cgf.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yzr.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xra.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://yjw.sufxvd.cn


<!-- 参考信息 -->