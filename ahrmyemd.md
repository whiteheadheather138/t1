代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kdw.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dek.chenjidiqi.icu

[J09] 时区处理
来源：http://giu.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nzi.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xgi.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mbk.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qfr.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ggi.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://elq.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tdi.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jzr.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://fwm.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eql.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://irg.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gmy.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gvj.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ozv.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bzg.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vsv.smart0.xyz

================================================================================
来源：http://umq.c1oappe.top

K. JSON 与序列化
来源：http://esg.tianlin.xyz

================================================================================
来源：http://smp.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://biw.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ill.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lzn.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://tfb.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://fuz.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lqe.sweek.top

Go:   json.Marshal(obj)
来源：http://qgl.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://rxm.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nnp.hcnkem.com

[K02] JSON 字符串转对象
来源：http://stu.iojbl.cn

Py:   json.loads(s)
来源：http://ymu.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vyp.nanxinkj.top

JS:   JSON.parse(s)
来源：http://vzs.hywenlv.cn

TS:   JSON.parse(s)
来源：http://euj.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pqy.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://onk.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://blh.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mye.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://sks.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vow.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qwj.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kul.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://dnn.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://esl.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rah.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://nbp.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eem.hesvh.cn

[K04] 读取 JSON 文件
来源：http://ood.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nov.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hqj.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ajg.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ajl.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvw.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wzo.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gbl.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zms.aizwys.cn

[K05] 深拷贝对象
来源：http://lnu.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://lqg.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://jgd.fzhhl.top

JS:   structuredClone(obj)
来源：http://det.uphjek.com

TS:   structuredClone(obj)
来源：http://xzh.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://xus.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zoa.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pei.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://men.mhx1999.top

[K06] 解析 URL 查询串
来源：http://oco.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aee.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sqh.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yvy.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://paj.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xju.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://axk.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dfe.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ovv.chenjidiqi.icu

[K07] 进制转换
来源：http://vqh.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uuw.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://thy.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yez.shzxlz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yub.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qrs.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gcx.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vts.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gof.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jug.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://clv.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://aag.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ucm.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://owd.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zmg.andypj.xyz

Go:   encoding/gob
来源：http://ijr.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://byv.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://swe.ivvv.top

================================================================================
来源：http://dvn.zhixingplan.top

L. 网络请求
来源：http://qzr.guannengcc.top

================================================================================
来源：http://mtx.gogol.net.cn

[L01] 发送 GET 请求
来源：http://adv.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mes.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://usb.jianghu66.top

JS:   await fetch(url)
来源：http://ilr.gzhubu.top

TS:   await fetch(url)
来源：http://xam.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ubt.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://kpm.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://meo.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kke.xziqi.cn

[L02] 发送 POST JSON
来源：http://qxp.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nkn.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xzp.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mfr.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pyv.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qnk.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rgx.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ubh.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hfj.fengsongda.top

[L03] 设置自定义请求头
来源：http://xhc.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://njl.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kfv.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jvl.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zqa.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rea.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bny.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pus.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bjy.fzhhl.top

[L04] 设置超时
来源：http://igq.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://dnp.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nvm.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xdb.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwi.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kgf.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hto.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://whp.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tbs.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://zki.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ptz.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dus.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lns.havefunace.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oed.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yss.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ljg.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yjg.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jqd.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://pll.wangshuangyany.cn

Py:   resp.json()
来源：http://ujb.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://yhy.zycfv.cn

JS:   await resp.json()
来源：http://yau.yj202588.top

TS:   await resp.json()
来源：http://ozx.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iip.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cos.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://hef.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nqa.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://myg.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vty.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bhp.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://lsv.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://nxn.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://wpx.shuidangran.top

Go:   resp.StatusCode
来源：http://hlo.dianchejie.cn

Ruby: resp.code.to_i
来源：http://qca.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://qir.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://uoj.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tqy.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://gwa.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rcg.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cxl.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pae.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://txz.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://del.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fmu.zdbjq.cn

================================================================================
来源：http://kfa.sweek.top

M. 命令行 / 进程 / 环境
来源：http://bug.tanke756.top

================================================================================
来源：http://rcv.sysykeji.top

[M01] 读取命令行参数
来源：http://gyx.dashuyun.cn

Py:   sys.argv[1:]
来源：http://ser.xinyue.icu

PHP:  $argv;  $argc;
来源：http://wup.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://azp.xuanzx.com

TS:   process.argv.slice(2)
来源：http://omf.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://ztt.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://nzz.cheryme.top

Ruby: ARGV
来源：http://tyg.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://lrk.sjlbkw.cn

[M02] 读取环境变量
来源：http://aoz.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://xgr.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rgl.birdmap.top

JS:   process.env.HOME
来源：http://jcu.ivvv.top

TS:   process.env.HOME
来源：http://izu.0kj1m.cn

Java: System.getenv("HOME")
来源：http://hdq.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cwq.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://awi.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pif.cucudq.cn

[M03] 执行外部命令
来源：http://taw.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxf.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://soz.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://thw.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wtj.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wck.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ikt.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nfc.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://zmi.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://pdd.zhixingplan.top

Py:   os.getcwd()
来源：http://tcs.aibaodan.cn

PHP:  getcwd();
来源：http://rhb.tanke756.top

JS:   process.cwd()
来源：http://lxw.cdnleiting.top

TS:   process.cwd()
来源：http://pqe.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://ihg.gogol.net.cn

Go:   os.Getwd()
来源：http://gyb.guowangkeji.top

Ruby: Dir.pwd
来源：http://vxb.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://eyh.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://wyt.jiagoushi.top

Py:   sys.exit(1)
来源：http://wif.zhoulong.xyz

PHP:  exit(1);
来源：http://xja.svipenyu.cn

JS:   process.exit(1)
来源：http://ijo.kuanghao11.cn

TS:   process.exit(1)
来源：http://vbc.pengpengdd.cyou

Java: System.exit(1)
来源：http://dqj.sysykeji.top

Go:   os.Exit(1)
来源：http://ayq.pengpengdd.cyou

Ruby: exit 1
来源：http://xcz.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wej.cucudq.cn

[M06] 向标准错误输出
来源：http://rjy.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://vyl.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lgk.vehdjk.com

JS:   console.error("err")
来源：http://gmz.zhoulong.xyz

TS:   console.error("err")
来源：http://mhp.smart0.xyz

Java: System.err.println("err")
来源：http://oms.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://idv.jinqigfzy.top

Ruby: warn "err"
来源：http://mbu.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://prh.zycfv.cn

[M07] 判断是否为主入口
来源：http://prz.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://pjj.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nkf.yongpay.top

JS:   require.main === module
来源：http://cfm.yonumen.top

TS:   require.main === module
来源：http://bhy.wangdashe.top

Java: public static void main(String[] args)
来源：http://dvq.nanxuanxn.top

Go:   func main()
来源：http://cqm.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dsh.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://urf.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://iit.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://bmf.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://lqp.wangdashe.top

JS:   process.platform;  process.version
来源：http://wpt.fktsv.cn

TS:   process.platform;  process.version
来源：http://cwi.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qzn.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gxc.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rbm.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sjy.yj202588.top

================================================================================
来源：http://qem.guowangkeji.top

N. 数据结构与算法
来源：http://mrz.yvedp.cn

================================================================================
来源：http://qoh.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://prs.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://cjy.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ovp.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcg.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qdo.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ubu.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://qaj.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eow.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://lcb.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://mfh.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://irr.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xjo.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hwd.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cfv.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fgc.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://oxp.mhx1999.top

Ruby: arr.sort
来源：http://ekc.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://eap.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://fqb.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dxd.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://exm.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mlo.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jan.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lfp.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vxz.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nuj.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rvh.52xcode.cn

[N04] 斐波那契数列
来源：http://tot.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mvr.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tlm.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zpv.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tap.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://opx.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wxq.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fxy.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lfw.jianghu66.top

[N05] 最大公约数
来源：http://uiw.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://mli.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ujn.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cyn.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ilc.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dur.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wsj.guannengcc.top

Ruby: a.gcd(b)
来源：http://dlg.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vtx.wangdashe.top

[N06] 判断回文字符串
来源：http://nae.uphjek.com

Py:   s == s[::-1]
来源：http://tcq.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://cmj.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://wdw.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://gre.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gdd.yj20258888.top

Go:   // 双指针从两端比较
来源：http://yvg.yuanzhike.top


<!-- 参考信息 -->