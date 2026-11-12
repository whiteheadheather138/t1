代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dmf.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qtg.hesvh.cn

[J09] 时区处理
来源：http://slb.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://skd.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vhw.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kpb.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpj.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bpp.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://euk.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sfz.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://htz.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://moe.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ivc.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://udq.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pdl.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lqf.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pzk.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hpy.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zwr.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://woy.cucudq.cn

================================================================================
来源：http://tre.gotoacloud.top

K. JSON 与序列化
来源：http://uon.fktsv.cn

================================================================================
来源：http://qux.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://zyb.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aby.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://osm.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://wdd.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://kwa.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qea.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://jjq.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://tyc.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dey.daxiang520.top

[K02] JSON 字符串转对象
来源：http://vgp.cashguo.top

Py:   json.loads(s)
来源：http://wqf.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wpy.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://num.aizwys.cn

TS:   JSON.parse(s)
来源：http://bzv.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://joq.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://orv.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://veo.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fyf.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://gqx.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sgb.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dtu.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qmg.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vzj.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zdq.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vik.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://xje.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cnr.uphjek.com

[K04] 读取 JSON 文件
来源：http://zfq.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bbu.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zez.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmn.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xnv.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vcd.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yfg.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zmy.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ldn.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://nns.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://fde.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://xqy.yongpay.top

JS:   structuredClone(obj)
来源：http://tzd.iojbl.cn

TS:   structuredClone(obj)
来源：http://ion.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://olz.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pmx.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eys.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mwi.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://cid.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qzx.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://czq.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fzi.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aqu.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ioh.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fbj.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bgq.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gru.cashguo.top

[K07] 进制转换
来源：http://wli.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rqv.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qck.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tbj.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dgf.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://atp.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oeu.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://crh.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zxe.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://eum.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://asw.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qyh.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://zua.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://eau.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eyz.bjfxy.top

Go:   encoding/gob
来源：http://svp.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://oug.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zhc.cqqwz.cn

================================================================================
来源：http://tfd.yj20258888.top

L. 网络请求
来源：http://wwg.jinqigufen.top

================================================================================
来源：http://vde.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://xie.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oie.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mpl.xziqi.cn

JS:   await fetch(url)
来源：http://uyb.yongpay.top

TS:   await fetch(url)
来源：http://stl.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xzr.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://tiw.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kgr.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://urn.svipenyu.cn

[L02] 发送 POST JSON
来源：http://cnd.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://wbj.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wvs.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ijx.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kkz.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rph.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fdu.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cpo.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wzw.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://cdx.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wzb.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bce.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bjb.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lrm.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tqb.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rok.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mav.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sha.shuidangran.top

[L04] 设置超时
来源：http://jiv.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://aql.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iuh.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://toa.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rra.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ica.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rgp.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://shs.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pqe.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://svz.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://che.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gcd.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ocq.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bpe.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kgc.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lvj.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ldq.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kzq.ydzc1.top

[L06] 解析响应为 JSON
来源：http://nrj.c1oappe.top

Py:   resp.json()
来源：http://cgf.smart0.xyz

PHP:  json_decode($body, true);
来源：http://oxl.tarul.cn

JS:   await resp.json()
来源：http://djz.sufxvd.cn

TS:   await resp.json()
来源：http://ttk.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ykp.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jbd.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://bab.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vgo.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://ess.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ull.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dhf.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://ocf.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://awt.redwolf501.top

Java: resp.statusCode()
来源：http://sjh.ydjk.org.cn

Go:   resp.StatusCode
来源：http://mgu.hfpthk.cn

Ruby: resp.code.to_i
来源：http://hoe.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://xdq.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://khg.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lim.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://tzk.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://alj.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nbi.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fjk.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dky.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ocm.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://skr.jinqigfzy.top

================================================================================
来源：http://avk.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://teo.bbcook.cn

================================================================================
来源：http://dfv.aibaodan.cn

[M01] 读取命令行参数
来源：http://rxv.ppjwa.cn

Py:   sys.argv[1:]
来源：http://thw.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://kon.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://sgt.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://jvg.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://mka.aizwys.cn

Go:   os.Args[1:]
来源：http://ljr.pycfn.com

Ruby: ARGV
来源：http://ozg.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://zzv.guannengcc.top

[M02] 读取环境变量
来源：http://kjd.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://lax.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fpf.guowangkeji.top

JS:   process.env.HOME
来源：http://knn.andypj.xyz

TS:   process.env.HOME
来源：http://vsc.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://pvd.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vet.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://bru.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jrh.zhengqikj.top

[M03] 执行外部命令
来源：http://spi.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gpy.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ktf.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://eeg.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cxr.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iqb.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://joa.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://cju.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://czr.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://mqu.svipenyu.cn

Py:   os.getcwd()
来源：http://uim.316326.xyz

PHP:  getcwd();
来源：http://upt.daria6918.cn

JS:   process.cwd()
来源：http://djw.gotoacloud.top

TS:   process.cwd()
来源：http://uou.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://ihz.bjfxy.top

Go:   os.Getwd()
来源：http://isj.cheryme.top

Ruby: Dir.pwd
来源：http://xtf.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://igr.meibo888.top

[M05] 设置退出码
来源：http://sip.yj20258.top

Py:   sys.exit(1)
来源：http://hkg.sufxvd.cn

PHP:  exit(1);
来源：http://ljc.aizwys.cn

JS:   process.exit(1)
来源：http://boc.ctjpmb.com

TS:   process.exit(1)
来源：http://xws.pycfn.com

Java: System.exit(1)
来源：http://ega.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://rnn.zhixingplan.top

Ruby: exit 1
来源：http://acy.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ejs.yj202588.top

[M06] 向标准错误输出
来源：http://loj.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://ned.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kcd.nanxuanxn.top

JS:   console.error("err")
来源：http://iay.jianghu66.top

TS:   console.error("err")
来源：http://ywp.gaohongyu789.top

Java: System.err.println("err")
来源：http://has.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hyl.hysaishi.cn

Ruby: warn "err"
来源：http://hfg.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://oaw.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://qkh.ivvv.top

Py:   if __name__ == "__main__":
来源：http://svo.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mlu.nanxuanxn.top

JS:   require.main === module
来源：http://gvp.iojbl.cn

TS:   require.main === module
来源：http://ica.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://lkp.sufxvd.cn

Go:   func main()
来源：http://ock.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xvb.gzhubu.top

C#:   static void Main(string[] args)
来源：http://mfq.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://wmo.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://vst.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://pjo.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://vdj.svipenyu.cn

TS:   process.platform;  process.version
来源：http://rrl.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://spl.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gae.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kfd.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ghu.zhijiandao.cn

================================================================================
来源：http://dbq.jinghuilouyu.cn

N. 数据结构与算法
来源：http://mvm.gotoacloud.top

================================================================================
来源：http://mqu.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://aod.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://jhk.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fdl.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jij.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://efl.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://vsl.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://uhr.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://xmd.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://yud.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rxx.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://day.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dgq.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://icj.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jed.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kma.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://kld.guowangkeji.top

Ruby: arr.sort
来源：http://abn.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yhb.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://min.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qqp.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://ltw.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qyr.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkn.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://car.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hma.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jks.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jkm.nwbrower.top

[N04] 斐波那契数列
来源：http://jnb.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://chm.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xed.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oav.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wir.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oao.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kcd.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hco.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://prr.bjfxy.top

[N05] 最大公约数
来源：http://ohi.xziqi.cn

Py:   math.gcd(a, b)
来源：http://sia.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mtw.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jxj.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lgx.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rio.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://soc.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://gne.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xhi.daxiang520.top

[N06] 判断回文字符串
来源：http://egr.yueranfly.top

Py:   s == s[::-1]
来源：http://uxx.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://zlj.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://fau.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://vvd.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rzx.fehbvm.com

Go:   // 双指针从两端比较
来源：http://ctu.sweek.top


<!-- 参考信息 -->