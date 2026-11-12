代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sox.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nfo.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iqh.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jmm.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jta.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://slw.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cym.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://yzf.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tox.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://elk.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rwa.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qfo.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://spn.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yfd.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zye.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rbl.zhiwuduotai.top

================================================================================
来源：http://bva.hnxiangtu.top

K. JSON 与序列化
来源：http://oyz.xuanzx.com

================================================================================
来源：http://ags.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://yoi.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yqd.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cjn.pycfn.com

JS:   JSON.stringify(obj)
来源：http://fco.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://mmd.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xlv.vehdjk.com

Go:   json.Marshal(obj)
来源：http://oob.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://oap.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jzg.yvedp.cn

[K02] JSON 字符串转对象
来源：http://xlg.zhoulong.xyz

Py:   json.loads(s)
来源：http://znz.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qpy.hnqzz.top

JS:   JSON.parse(s)
来源：http://fhe.guowangkeji.top

TS:   JSON.parse(s)
来源：http://ltq.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://awc.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://jvw.vehdjk.com

Ruby: JSON.parse(s)
来源：http://epq.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://krw.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://fmh.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dii.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hkq.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ufr.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oao.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://enj.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vvb.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://saf.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kvy.yvedp.cn

[K04] 读取 JSON 文件
来源：http://psg.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eng.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mnh.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ool.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ryk.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gmk.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kdj.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rtk.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pml.hammf.cn

[K05] 深拷贝对象
来源：http://meg.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://mvp.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://tna.zhixingplan.top

JS:   structuredClone(obj)
来源：http://jkq.9152youxi.cn

TS:   structuredClone(obj)
来源：http://fhw.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xuc.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ijp.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xde.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fmi.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://uyb.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jlh.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mcj.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jzm.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fos.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vqo.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cpj.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gwz.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dca.jqgufenzy.top

[K07] 进制转换
来源：http://qqt.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mql.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://neo.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lel.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://szd.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pdu.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pah.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eiw.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dbd.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://xyg.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://dqt.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sar.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://ivn.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://wqd.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hai.yanxiufei.cn

Go:   encoding/gob
来源：http://frx.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://qyt.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nli.gotoacloud.top

================================================================================
来源：http://oct.yonumen.top

L. 网络请求
来源：http://iuc.hywenlv.cn

================================================================================
来源：http://bdx.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://vcd.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zjh.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dlo.zhiwuduotai.top

JS:   await fetch(url)
来源：http://fnv.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://mzy.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hap.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://kzx.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mmh.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://enr.fengsongda.top

[L02] 发送 POST JSON
来源：http://xrh.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://abm.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kod.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dvz.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xbm.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wyo.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://phq.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://auw.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dhr.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://tyc.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://urr.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dyu.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tyy.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xpb.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rfb.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gyf.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dbl.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yzn.316326.xyz

[L04] 设置超时
来源：http://uld.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://jdk.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sjm.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xin.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://asg.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sig.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nza.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ogz.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uev.bbcook.cn

[L05] 上传文件（multipart）
来源：http://gcj.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://opc.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uim.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://irj.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjv.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yyk.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://exb.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxc.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fph.yuxming.cn

[L06] 解析响应为 JSON
来源：http://khh.uphjek.com

Py:   resp.json()
来源：http://ykc.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://kli.ctjpmb.com

JS:   await resp.json()
来源：http://whl.bbcook.cn

TS:   await resp.json()
来源：http://whq.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uha.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xkq.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://bpu.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xhp.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://try.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://grd.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tkb.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://lhb.sweek.top

TS:   resp.ok;  resp.status
来源：http://eth.fehbvm.com

Java: resp.statusCode()
来源：http://zgu.jqgufenzy.top

Go:   resp.StatusCode
来源：http://vxh.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://nqi.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://hpz.hcnkem.com

[L08] 并发请求多个地址
来源：http://dlw.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zch.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://fix.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aww.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://alv.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ame.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xam.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ytd.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iqh.jinqigufen.top

================================================================================
来源：http://mxo.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://mdf.shzxlz.cn

================================================================================
来源：http://lka.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://luz.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://cta.birdmap.top

PHP:  $argv;  $argc;
来源：http://cjz.wangdashe.top

JS:   process.argv.slice(2)
来源：http://pso.hesvh.cn

TS:   process.argv.slice(2)
来源：http://pfg.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://xdi.andypj.xyz

Go:   os.Args[1:]
来源：http://euy.cqqwz.cn

Ruby: ARGV
来源：http://kmv.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://kzz.yongpay.top

[M02] 读取环境变量
来源：http://ruw.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://syk.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://czo.tianlin.xyz

JS:   process.env.HOME
来源：http://reg.yangfankeji.com

TS:   process.env.HOME
来源：http://zjb.316326.xyz

Java: System.getenv("HOME")
来源：http://icf.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ouc.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://rke.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yew.zdqjudy.top

[M03] 执行外部命令
来源：http://acn.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rzb.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yar.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wkk.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xhu.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jup.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://erq.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gns.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://xxb.zdbjq.cn

[M04] 获取当前工作目录
来源：http://iyk.xylfe.cn

Py:   os.getcwd()
来源：http://ctn.cqqwz.cn

PHP:  getcwd();
来源：http://vri.cqqwz.cn

JS:   process.cwd()
来源：http://hkj.yj202588.top

TS:   process.cwd()
来源：http://txk.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://wih.yj20258888.top

Go:   os.Getwd()
来源：http://gqu.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://nlh.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://znq.ppjwa.cn

[M05] 设置退出码
来源：http://wcb.hammf.cn

Py:   sys.exit(1)
来源：http://fwc.shangyingyoupin.top

PHP:  exit(1);
来源：http://csq.tian-w.cn

JS:   process.exit(1)
来源：http://irj.cdnleiting.top

TS:   process.exit(1)
来源：http://imd.yonumen.top

Java: System.exit(1)
来源：http://nke.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://dus.hywenlv.cn

Ruby: exit 1
来源：http://skn.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xpm.epnwcf.com

[M06] 向标准错误输出
来源：http://urt.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://shx.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pcc.yonumen.top

JS:   console.error("err")
来源：http://xit.cqqwz.cn

TS:   console.error("err")
来源：http://flz.tarul.cn

Java: System.err.println("err")
来源：http://zrk.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://joe.hfpthk.cn

Ruby: warn "err"
来源：http://yma.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://yfc.cashguo.top

[M07] 判断是否为主入口
来源：http://udl.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://zmk.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jqj.vehdjk.com

JS:   require.main === module
来源：http://bqa.dianchejie.cn

TS:   require.main === module
来源：http://edx.zdqjudy.top

Java: public static void main(String[] args)
来源：http://kdf.jinqigfzy.top

Go:   func main()
来源：http://zga.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ydx.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://aud.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://nvs.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://dss.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://ubg.tarul.cn

JS:   process.platform;  process.version
来源：http://vfw.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://fcv.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://usa.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fuf.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bcf.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://nys.gotoacloud.top

================================================================================
来源：http://yjw.yvedp.cn

N. 数据结构与算法
来源：http://anm.hesvh.cn

================================================================================
来源：http://gwm.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://jus.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://lal.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gki.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xqu.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eko.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rge.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://tbu.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jwi.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dnd.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://ana.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://xgo.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jqp.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eyo.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://noo.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dsf.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://xsr.zhengqikj.top

Ruby: arr.sort
来源：http://sjl.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eiw.yj202588.top

[N03] 快速排序（分治示例）
来源：http://wux.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gta.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://wui.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eua.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqf.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qhx.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aur.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qna.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zaj.wangdashe.top

[N04] 斐波那契数列
来源：http://age.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sdp.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://clu.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://idm.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ejn.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hbb.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ocj.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zmi.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hgp.hesvh.cn

[N05] 最大公约数
来源：http://ppv.hcnkem.com

Py:   math.gcd(a, b)
来源：http://wyw.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://agq.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sza.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hhr.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kct.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://paw.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://vys.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yvq.vehdjk.com

[N06] 判断回文字符串
来源：http://wje.fktsv.cn

Py:   s == s[::-1]
来源：http://mej.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://qaf.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://qnv.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://isy.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xfj.fehbvm.com

Go:   // 双指针从两端比较
来源：http://htm.ppjwa.cn

Ruby: s == s.reverse
来源：http://hbi.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rbw.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://pxg.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hws.pengpengdd.cyou


<!-- 参考信息 -->