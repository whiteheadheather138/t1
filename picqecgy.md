代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jme.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bzm.xuanzx.com

[J09] 时区处理
来源：http://ole.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mpo.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mup.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://byy.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zcz.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pcx.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vct.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tci.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jme.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://rlq.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hnx.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lus.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wta.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://njo.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mdt.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jik.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pld.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pqy.vqdsnc.cn

================================================================================
来源：http://jqd.tanke756.top

K. JSON 与序列化
来源：http://cza.xziqi.cn

================================================================================
来源：http://vwe.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://esy.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvj.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xjj.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://pjy.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://ilv.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ash.yj20258888.top

Go:   json.Marshal(obj)
来源：http://njc.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://ksf.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tvs.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://ofq.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://sda.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qdx.cucudq.cn

JS:   JSON.parse(s)
来源：http://sxf.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://byj.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tue.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://iof.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://mwm.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://boh.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://ryx.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zuq.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mjz.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://iki.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ykl.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://izi.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xvo.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://zos.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://evw.sxryk.cn

[K04] 读取 JSON 文件
来源：http://ycr.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ugq.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dds.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://axj.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xfs.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ovp.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cxk.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qwn.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iyp.yj202588.top

[K05] 深拷贝对象
来源：http://gfu.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://mhy.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://afe.yvedp.cn

JS:   structuredClone(obj)
来源：http://gak.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://zow.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tgp.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aiw.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vsg.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vam.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://sqi.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vvy.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mlf.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xdv.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgz.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nbl.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://npw.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://utv.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iyp.ivvv.top

[K07] 进制转换
来源：http://fpu.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dht.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bwo.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lhf.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yqs.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bir.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tcj.zhaomingkeji.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ptx.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hff.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://ohb.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://fqx.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pxu.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://sgd.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://vin.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yod.hcnkem.com

Go:   encoding/gob
来源：http://lpz.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://pwg.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hmv.jqgufenzy.top

================================================================================
来源：http://eqb.daria6918.cn

L. 网络请求
来源：http://ttb.yj202588.top

================================================================================
来源：http://bsh.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://rvo.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wvt.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tkv.yueranfly.top

JS:   await fetch(url)
来源：http://png.hysaishi.cn

TS:   await fetch(url)
来源：http://ejy.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zuj.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://ouz.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wnx.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bvg.aizwys.cn

[L02] 发送 POST JSON
来源：http://liw.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oex.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nhe.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ank.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ujw.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://els.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ewk.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mcu.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zob.tianlin.xyz

[L03] 设置自定义请求头
来源：http://xtj.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aaf.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lfm.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://orx.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qxd.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sla.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gvc.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ddc.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ard.kuanghao11.cn

[L04] 设置超时
来源：http://cul.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://drl.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lyh.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jay.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lsa.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dii.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mgj.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qtk.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yj20258.top

[L05] 上传文件（multipart）
来源：http://fkp.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bxn.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rpo.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xbe.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nvq.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hzs.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dbd.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vbd.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ujp.yongpay.top

[L06] 解析响应为 JSON
来源：http://wat.snrcjt.cn

Py:   resp.json()
来源：http://lbk.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://erx.yfazqb.com

JS:   await resp.json()
来源：http://gbe.jyoumei.cn

TS:   await resp.json()
来源：http://dyn.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://atb.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://thu.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://lgw.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lxb.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://qcs.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nin.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qiu.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://ffa.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://fng.ehwqpu.com

Java: resp.statusCode()
来源：http://dwc.shzxlz.cn

Go:   resp.StatusCode
来源：http://ejm.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://lnc.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://jyx.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://zjm.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://atr.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://okf.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qvc.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcr.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wpg.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tbf.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ksk.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ewh.c1oappe.top

================================================================================
来源：http://ssl.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://pko.zdqjudy.top

================================================================================
来源：http://ntj.quarkkingdee.top

[M01] 读取命令行参数
来源：http://avh.gzhubu.top

Py:   sys.argv[1:]
来源：http://mkg.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://kkt.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://chp.redwolf501.top

TS:   process.argv.slice(2)
来源：http://ygu.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://xyc.ydzc1.top

Go:   os.Args[1:]
来源：http://lbh.zhoulong.xyz

Ruby: ARGV
来源：http://ynf.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://isp.hysaishi.cn

[M02] 读取环境变量
来源：http://eyi.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://xgx.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vcb.yvedp.cn

JS:   process.env.HOME
来源：http://aof.fehbvm.com

TS:   process.env.HOME
来源：http://gld.vehdjk.com

Java: System.getenv("HOME")
来源：http://rvp.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bsu.xylfe.cn

Ruby: ENV["HOME"]
来源：http://nxz.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jtj.ivvv.top

[M03] 执行外部命令
来源：http://foy.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uzu.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iga.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://acz.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tjy.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vma.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xkp.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://uhd.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://lpc.zycfv.cn

[M04] 获取当前工作目录
来源：http://upa.dianchejie.cn

Py:   os.getcwd()
来源：http://snu.jyoumei.cn

PHP:  getcwd();
来源：http://kfm.hammf.cn

JS:   process.cwd()
来源：http://xks.yueranfly.top

TS:   process.cwd()
来源：http://klg.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://fyi.guannengcc.top

Go:   os.Getwd()
来源：http://dja.tarul.cn

Ruby: Dir.pwd
来源：http://bdm.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mst.sjlbkw.cn

[M05] 设置退出码
来源：http://snf.cheryme.top

Py:   sys.exit(1)
来源：http://hjq.zycfv.cn

PHP:  exit(1);
来源：http://vws.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://zug.hnqzz.top

TS:   process.exit(1)
来源：http://tit.meibo888.top

Java: System.exit(1)
来源：http://pef.9152youxi.cn

Go:   os.Exit(1)
来源：http://mrf.shzxlz.cn

Ruby: exit 1
来源：http://jbp.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gmt.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://jcr.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://fcc.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://hve.yj20258888.top

JS:   console.error("err")
来源：http://xkz.fanxiaobao.xyz

TS:   console.error("err")
来源：http://dgd.gogol.net.cn

Java: System.err.println("err")
来源：http://jnx.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pby.havefunace.top

Ruby: warn "err"
来源：http://phe.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://yem.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://ahu.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://ira.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xsn.hywenlv.cn

JS:   require.main === module
来源：http://usf.epnwcf.com

TS:   require.main === module
来源：http://obg.fzhhl.top

Java: public static void main(String[] args)
来源：http://hfj.yfazqb.com

Go:   func main()
来源：http://ccs.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ckd.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://jdg.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://nhp.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://cej.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://bcm.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://mnp.snrcjt.cn

TS:   process.platform;  process.version
来源：http://aej.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ckf.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ync.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://irk.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xzi.cheryme.top

================================================================================
来源：http://xwc.sweek.top

N. 数据结构与算法
来源：http://yhn.wangdashe.top

================================================================================
来源：http://fvv.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://hrk.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zzc.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mqg.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://axl.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ugl.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oor.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://doz.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vmt.mhx1999.top

C#:   Array.BinarySearch(arr, x)
来源：http://vlg.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://yuq.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://lcu.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://akz.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kkr.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://mtu.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zdh.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://gbh.zycfv.cn

Ruby: arr.sort
来源：http://cxg.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://apg.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://pli.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uzt.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://bob.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iqd.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yfu.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://msf.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kvm.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ghs.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hgf.tianlin.xyz

[N04] 斐波那契数列
来源：http://edj.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://deo.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xlu.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mpq.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rov.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tol.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jic.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://thp.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eat.jyoumei.cn

[N05] 最大公约数
来源：http://hxy.wangdashe.top

Py:   math.gcd(a, b)
来源：http://ibc.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ajl.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://njv.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ysc.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tae.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cqu.bbcook.cn

Ruby: a.gcd(b)
来源：http://qlf.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rcj.0kj1m.cn

[N06] 判断回文字符串
来源：http://nzx.yonumen.top

Py:   s == s[::-1]
来源：http://exx.ybcxt.top

PHP:  $s === strrev($s);
来源：http://bwx.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://miv.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://dkr.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lib.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://mnr.bbcook.cn


<!-- 参考信息 -->