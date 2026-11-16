代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cmq.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://egc.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cfd.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iqd.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://scv.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hob.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uzf.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://kgr.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ile.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://plh.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aqr.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://asx.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kdq.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bkl.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://los.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://agb.fzhhl.top

================================================================================
来源：http://udn.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://hhc.gzhubu.top

================================================================================
来源：http://ztk.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://sol.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zrg.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kal.cheryme.top

JS:   JSON.stringify(obj)
来源：http://gfc.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://jqx.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ypz.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://ldn.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://ixk.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xbl.ybcxt.top

[K02] JSON 字符串转对象
来源：http://fps.zdqjudy.top

Py:   json.loads(s)
来源：http://tma.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cic.yuxming.cn

JS:   JSON.parse(s)
来源：http://xgq.yj202588.top

TS:   JSON.parse(s)
来源：http://zmj.andypj.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://srs.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://jnq.daria6918.cn

Ruby: JSON.parse(s)
来源：http://lwt.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://amt.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://yws.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pie.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fdl.uphjek.com

JS:   JSON.stringify(obj, null, 2)
来源：http://zuc.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sok.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aez.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qen.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aot.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gss.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://sad.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fek.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mnq.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rdp.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pkq.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://brl.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lnr.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dhj.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cqo.guowangkeji.top

[K05] 深拷贝对象
来源：http://cio.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://vod.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://fsp.tian-w.cn

JS:   structuredClone(obj)
来源：http://pjn.gotoacloud.top

TS:   structuredClone(obj)
来源：http://hwb.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nyo.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://guf.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qdi.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hon.sysykeji.top

[K06] 解析 URL 查询串
来源：http://mqh.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bpn.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hhr.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xut.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yma.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://use.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://bdm.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mqc.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vla.quarkkingdee.top

[K07] 进制转换
来源：http://noc.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vqp.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qpi.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wzh.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dvy.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://snk.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ykl.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wyg.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zba.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://ddf.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://ahw.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tso.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://kgu.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://kzp.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jab.jqgfzy.top

Go:   encoding/gob
来源：http://bck.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://zda.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://laq.aibaodan.cn

================================================================================
来源：http://fut.nanxuanxn.top

L. 网络请求
来源：http://lqz.epnwcf.com

================================================================================
来源：http://cse.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://qhz.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cqx.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ywr.jiagoushi.top

JS:   await fetch(url)
来源：http://jhb.meibo888.top

TS:   await fetch(url)
来源：http://nto.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kut.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://etl.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jxu.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pue.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://hhr.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eef.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fig.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fqe.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://svc.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rjt.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qxe.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hrh.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://don.iojbl.cn

[L03] 设置自定义请求头
来源：http://okn.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qrq.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vyt.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fiq.tian-w.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rjj.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rad.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bpm.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rpg.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://emh.zhiwuduotai.top

[L04] 设置超时
来源：http://jpm.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://dau.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rsh.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hgm.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bhf.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nvb.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cjh.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aum.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sxc.epnwcf.com

[L05] 上传文件（multipart）
来源：http://byx.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zzh.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rel.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dsx.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mnx.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gsb.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ago.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kpk.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wxi.bjfxy.top

[L06] 解析响应为 JSON
来源：http://wbh.sysykeji.top

Py:   resp.json()
来源：http://tyb.bjfxy.top

PHP:  json_decode($body, true);
来源：http://ivm.havefunace.top

JS:   await resp.json()
来源：http://fhu.cheryme.top

TS:   await resp.json()
来源：http://wnp.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ure.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xbf.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://khw.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wph.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://nun.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xbr.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ins.cheryme.top

JS:   resp.ok;  resp.status
来源：http://zwf.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://yjo.guowangkeji.top

Java: resp.statusCode()
来源：http://pus.wangdashe.top

Go:   resp.StatusCode
来源：http://qab.jiagoushi.top

Ruby: resp.code.to_i
来源：http://abq.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://efi.sysykeji.top

[L08] 并发请求多个地址
来源：http://rxt.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bcw.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://ajr.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sdv.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ghz.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uvh.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jpq.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zow.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kpu.yj20258.top

================================================================================
来源：http://ywz.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://zcs.gzhubu.top

================================================================================
来源：http://qkl.yueranfly.top

[M01] 读取命令行参数
来源：http://iyc.epnwcf.com

Py:   sys.argv[1:]
来源：http://cjc.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://kdu.cucudq.cn

JS:   process.argv.slice(2)
来源：http://txf.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://wds.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://mos.hnqzz.top

Go:   os.Args[1:]
来源：http://nmg.sweek.top

Ruby: ARGV
来源：http://kmq.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://qsv.yuanzhike.top

[M02] 读取环境变量
来源：http://enm.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://ruk.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://epu.birdmap.top

JS:   process.env.HOME
来源：http://apq.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://uky.mhx1999.top

Java: System.getenv("HOME")
来源：http://edl.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dui.zhaomingkeji.xyz

Ruby: ENV["HOME"]
来源：http://arg.jinqigfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hjp.fehbvm.com

[M03] 执行外部命令
来源：http://jmd.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vxx.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pos.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://utb.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://rpk.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://met.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://koo.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gke.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://sqf.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://viq.sxryk.cn

Py:   os.getcwd()
来源：http://web.chenlongwang.top

PHP:  getcwd();
来源：http://zkd.hammf.cn

JS:   process.cwd()
来源：http://ght.gzhubu.top

TS:   process.cwd()
来源：http://xaf.jiagoushi.top

Java: Path.of("").toAbsolutePath()
来源：http://vjj.birdmap.top

Go:   os.Getwd()
来源：http://bvv.sysykeji.top

Ruby: Dir.pwd
来源：http://vgo.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://utx.jiagoushi.top

[M05] 设置退出码
来源：http://lsk.vqdsnc.cn

Py:   sys.exit(1)
来源：http://xvb.fehbvm.com

PHP:  exit(1);
来源：http://rtj.hywenlv.cn

JS:   process.exit(1)
来源：http://sgl.vehdjk.com

TS:   process.exit(1)
来源：http://ggf.dianchejie.cn

Java: System.exit(1)
来源：http://civ.dashuyun.cn

Go:   os.Exit(1)
来源：http://awx.tianlin.xyz

Ruby: exit 1
来源：http://ksu.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uyq.snrcjt.cn

[M06] 向标准错误输出
来源：http://gub.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://ptq.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hms.hcnkem.com

JS:   console.error("err")
来源：http://hpy.jqgufenzy.top

TS:   console.error("err")
来源：http://rgi.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://qym.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://srq.shzxlz.cn

Ruby: warn "err"
来源：http://mtf.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://wfz.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://jjm.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://pvj.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jxs.yj20258888.top

JS:   require.main === module
来源：http://rmw.ywan-chungtsiang.top

TS:   require.main === module
来源：http://mpd.sweek.top

Java: public static void main(String[] args)
来源：http://iux.shuidangran.top

Go:   func main()
来源：http://int.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qxn.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://qhy.birdmap.top

[M08] 获取系统与运行时信息
来源：http://hna.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://jzt.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://udk.cdnleiting.top

JS:   process.platform;  process.version
来源：http://wys.zycfv.cn

TS:   process.platform;  process.version
来源：http://haw.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rem.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pgk.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bwi.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lur.zhiwuduotai.top

================================================================================
来源：http://zuh.iojbl.cn

N. 数据结构与算法
来源：http://bro.jinqigfzy.top

================================================================================
来源：http://gpx.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://nmp.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://lhl.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yqt.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bsa.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lbc.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://avh.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://nsm.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ryu.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://lno.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://gjk.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://fxa.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jjl.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xlo.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yrp.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kyr.bbcook.cn

Go:   slices.Sort(arr)
来源：http://khe.epnwcf.com

Ruby: arr.sort
来源：http://fws.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nbt.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://oqp.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fwe.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://lxy.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ink.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cuz.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lrc.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://edr.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jjs.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://vxm.quarkkingdee.top

[N04] 斐波那契数列
来源：http://jot.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wql.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qon.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yuf.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://phn.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hig.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rcb.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mkd.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zkz.yuanzhike.top

[N05] 最大公约数
来源：http://kgb.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://kyb.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://unz.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hoz.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ygc.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mbi.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://goy.chenlongwang.top

Ruby: a.gcd(b)
来源：http://lyx.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qqp.ivvv.top

[N06] 判断回文字符串
来源：http://gay.cdnleiting.top

Py:   s == s[::-1]
来源：http://uhg.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://ujy.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://nxx.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://hqc.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ygj.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://mfs.iojbl.cn

Ruby: s == s.reverse
来源：http://wja.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jny.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://jqx.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kbk.cashguo.top


<!-- 参考信息 -->