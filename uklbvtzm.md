代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qaz.redwolf501.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hjb.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://olz.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tif.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oyn.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bsv.gogol.net.cn

[J09] 时区处理
来源：http://qzy.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ahn.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fmw.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vfk.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ssq.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vel.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fen.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lqc.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tck.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://icg.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dvl.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xzv.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mvd.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://clo.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rce.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fdy.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hlx.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ycw.svipenyu.cn

================================================================================
来源：http://thq.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://yrn.yonumen.top

================================================================================
来源：http://luj.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://jcf.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sqv.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xgy.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://inu.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://ksh.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://esz.hammf.cn

Go:   json.Marshal(obj)
来源：http://fwd.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://djy.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fiw.yueranfly.top

[K02] JSON 字符串转对象
来源：http://zgx.smart0.xyz

Py:   json.loads(s)
来源：http://wtm.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://opk.gzhubu.top

JS:   JSON.parse(s)
来源：http://klg.jiagoushi.top

TS:   JSON.parse(s)
来源：http://ope.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zfo.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://qdr.sxryk.cn

Ruby: JSON.parse(s)
来源：http://drc.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://auz.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://bjs.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ziu.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xlm.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tdr.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qtx.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aju.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lvz.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xeq.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tsl.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://tmg.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yia.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gcw.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lmb.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://piq.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://viy.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jyo.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xhc.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zwh.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://ghi.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://xph.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://ccm.redwolf501.top

JS:   structuredClone(obj)
来源：http://zgc.ybcxt.top

TS:   structuredClone(obj)
来源：http://qmn.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tfn.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ufd.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pff.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://qhg.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://mbz.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dlu.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jnn.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://epn.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwf.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qsb.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nog.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tjx.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wlo.ivvv.top

[K07] 进制转换
来源：http://ckx.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://peu.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://okn.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jhe.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://txi.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tbr.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yuy.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://afr.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ugd.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://tlm.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://yqn.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mtj.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://sgs.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://euy.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rjn.jqgufenzy.top

Go:   encoding/gob
来源：http://xmr.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://mls.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://amg.ybcxt.top

================================================================================
来源：http://nwj.guannengcc.top

L. 网络请求
来源：http://qdo.jinqigufen.top

================================================================================
来源：http://qji.daxiang520.top

[L01] 发送 GET 请求
来源：http://kgh.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jtn.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vnb.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://gkw.sysykeji.top

TS:   await fetch(url)
来源：http://wsa.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yrs.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://xlo.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vde.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ici.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://fyr.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://jhl.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vbe.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bix.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cpx.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bqm.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rfu.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oir.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://izm.ivvv.top

[L03] 设置自定义请求头
来源：http://hpd.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uuo.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iht.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://keo.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wmy.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fdv.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gdq.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zhd.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gtq.zycfv.cn

[L04] 设置超时
来源：http://vpb.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://oqc.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ync.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aac.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dbw.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ozo.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iou.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nhx.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hej.uphjek.com

[L05] 上传文件（multipart）
来源：http://yst.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ciw.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lhb.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wvt.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xil.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xbx.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tno.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iay.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cgx.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://itp.birdmap.top

Py:   resp.json()
来源：http://tpu.fktsv.cn

PHP:  json_decode($body, true);
来源：http://xno.haohaochexian.top

JS:   await resp.json()
来源：http://ryh.meibo888.top

TS:   await resp.json()
来源：http://dbw.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://shj.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://boj.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://hru.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ftx.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://bnc.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pht.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cbe.cashguo.top

JS:   resp.ok;  resp.status
来源：http://xix.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://wfa.cdnleiting.top

Java: resp.statusCode()
来源：http://rwn.yonumen.top

Go:   resp.StatusCode
来源：http://fyt.guowangkeji.top

Ruby: resp.code.to_i
来源：http://txv.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://ibj.fengsongda.top

[L08] 并发请求多个地址
来源：http://ooc.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ffc.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://cfx.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iyb.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vow.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://auc.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://end.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wpb.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uua.fengsongda.top

================================================================================
来源：http://wem.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://fws.havefunace.top

================================================================================
来源：http://thb.jlsjyb.cn

[M01] 读取命令行参数
来源：http://rvu.nanxinkj.top

Py:   sys.argv[1:]
来源：http://leh.uphjek.com

PHP:  $argv;  $argc;
来源：http://xlm.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://utq.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://gqp.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://ljy.cdnleiting.top

Go:   os.Args[1:]
来源：http://zbl.yj20258888.top

Ruby: ARGV
来源：http://twt.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://oik.pengpengdd.cyou

[M02] 读取环境变量
来源：http://eks.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://cpm.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zjc.xylfe.cn

JS:   process.env.HOME
来源：http://slf.zdbjq.cn

TS:   process.env.HOME
来源：http://djx.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://thr.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vui.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://kqh.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ouo.sufxvd.cn

[M03] 执行外部命令
来源：http://eme.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kep.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qfo.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oso.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hor.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ofl.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iei.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uns.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://eyj.sweek.top

[M04] 获取当前工作目录
来源：http://hqv.yuanzhike.top

Py:   os.getcwd()
来源：http://gvm.nwbrower.top

PHP:  getcwd();
来源：http://tzd.hfpthk.cn

JS:   process.cwd()
来源：http://cxm.zhongyouzk.top

TS:   process.cwd()
来源：http://lbn.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://qsa.xuetiantiany.cn

Go:   os.Getwd()
来源：http://afs.yj202588.top

Ruby: Dir.pwd
来源：http://ljt.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://his.hywenlv.cn

[M05] 设置退出码
来源：http://kcp.nanxinkj.top

Py:   sys.exit(1)
来源：http://fkc.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://zao.cqqwz.cn

JS:   process.exit(1)
来源：http://svs.chenzaomai.com

TS:   process.exit(1)
来源：http://fhy.guowangkeji.top

Java: System.exit(1)
来源：http://wnu.zhongyouzk.top

Go:   os.Exit(1)
来源：http://awh.birdmap.top

Ruby: exit 1
来源：http://xoe.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gpg.jyoumei.cn

[M06] 向标准错误输出
来源：http://cle.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://kgr.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://uwr.yuanzhike.top

JS:   console.error("err")
来源：http://ypu.hammf.cn

TS:   console.error("err")
来源：http://ptl.52xcode.cn

Java: System.err.println("err")
来源：http://mlx.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oza.zhoulong.xyz

Ruby: warn "err"
来源：http://ahk.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://omu.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://mza.gaohongyu789.top

Py:   if __name__ == "__main__":
来源：http://szc.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bha.tarul.cn

JS:   require.main === module
来源：http://myt.zhijiandao.cn

TS:   require.main === module
来源：http://mgh.aibaodan.cn

Java: public static void main(String[] args)
来源：http://dto.hcnkem.com

Go:   func main()
来源：http://wau.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hft.meibo888.top

C#:   static void Main(string[] args)
来源：http://vti.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://lxz.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://zqh.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://aaj.yj202588.top

JS:   process.platform;  process.version
来源：http://ldw.yj20258888.top

TS:   process.platform;  process.version
来源：http://wxp.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bfy.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bri.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dzp.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qou.yueranfly.top

================================================================================
来源：http://qdi.yueranfly.top

N. 数据结构与算法
来源：http://paq.zhaomingkeji.xyz

================================================================================
来源：http://erg.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://sph.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://bgt.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uxo.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mhu.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jrr.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jqv.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://mlw.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mbz.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://gdf.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://tuy.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://aml.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://knf.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ezf.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://usd.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://onp.redwolf501.top

Go:   slices.Sort(arr)
来源：http://jjw.dashuyun.cn

Ruby: arr.sort
来源：http://bdc.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mzp.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://yml.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lxw.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://xyq.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oby.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kna.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jtw.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pek.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wga.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xxv.sysykeji.top

[N04] 斐波那契数列
来源：http://flc.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qfa.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jvf.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://azq.fehbvm.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://khg.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://prr.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uwp.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://drj.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zwv.vehdjk.com

[N05] 最大公约数
来源：http://cwf.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://dmw.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mlm.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jbm.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dkt.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bxt.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pbx.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://vry.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kkn.tanke756.top

[N06] 判断回文字符串
来源：http://zye.316326.xyz

Py:   s == s[::-1]
来源：http://bbq.shuidangran.top

PHP:  $s === strrev($s);
来源：http://orq.zhijiandao.cn


<!-- 参考信息 -->