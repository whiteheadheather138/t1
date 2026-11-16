代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tvc.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yzt.chenjidiqi.icu

[J09] 时区处理
来源：http://som.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://amt.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sog.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://coi.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sfi.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fty.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://znq.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yaw.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://myb.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://wog.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ozo.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gjl.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://znb.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://div.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xav.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oma.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bmb.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cab.hnqzz.top

================================================================================
来源：http://mtv.fehbvm.com

K. JSON 与序列化
来源：http://yxr.yj20258.top

================================================================================
来源：http://etn.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://iun.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://plz.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://znz.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://ebz.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://kkg.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jqo.yj202588.top

Go:   json.Marshal(obj)
来源：http://ibq.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://spx.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://myd.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://iil.meibo888.top

Py:   json.loads(s)
来源：http://blz.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wdb.tianlin.xyz

JS:   JSON.parse(s)
来源：http://shh.daria6918.cn

TS:   JSON.parse(s)
来源：http://asa.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kqa.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://gsp.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://sqy.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ere.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://yxw.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://etl.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ull.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fqb.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://lph.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nvz.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fva.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uzu.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tph.tian-w.cn

[K04] 读取 JSON 文件
来源：http://vpg.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oik.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cwn.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujy.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vkz.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ozv.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xdl.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://tvc.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yta.daxiang520.top

[K05] 深拷贝对象
来源：http://brj.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://etm.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://rpm.yonumen.top

JS:   structuredClone(obj)
来源：http://inh.redwolf501.top

TS:   structuredClone(obj)
来源：http://ogq.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vbj.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pjl.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dbt.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tth.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://kcr.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yvn.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pqc.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfy.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://twd.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rsu.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wrp.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vvx.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ovq.wangdashe.top

[K07] 进制转换
来源：http://fdi.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pwg.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cre.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ujd.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aeq.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fvi.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gxl.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nkd.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://smx.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://pqc.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://frf.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iuk.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://kgn.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://zie.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ltr.zhongyouzk.top

Go:   encoding/gob
来源：http://nix.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://cka.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://etf.jiagoushi.top

================================================================================
来源：http://mbd.yj202588.top

L. 网络请求
来源：http://ijd.redwolf501.top

================================================================================
来源：http://icj.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://fob.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qro.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nvg.feifeiyinyue.top

JS:   await fetch(url)
来源：http://xlg.aizwys.cn

TS:   await fetch(url)
来源：http://kmm.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ump.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://lbl.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://koh.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uoq.yongpay.top

[L02] 发送 POST JSON
来源：http://tkf.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://ftz.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tzz.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zez.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://btj.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cox.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mva.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://clm.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qdf.jianghu66.top

[L03] 设置自定义请求头
来源：http://wjw.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hhg.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kqb.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bhb.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgz.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fry.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gjy.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rht.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uiw.sxryk.cn

[L04] 设置超时
来源：http://act.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://vdz.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zxm.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://itb.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nxd.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ppz.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gau.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://plj.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qsb.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://lni.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gvt.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fam.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vzt.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xlu.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hhn.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bai.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rxe.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rvf.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://top.yueranfly.top

Py:   resp.json()
来源：http://puu.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://jqb.316326.xyz

JS:   await resp.json()
来源：http://wig.pycfn.com

TS:   await resp.json()
来源：http://gws.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vyj.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gxs.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://ttd.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bcn.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://sgm.tianlin.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ntc.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cth.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://ods.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://lso.xylfe.cn

Java: resp.statusCode()
来源：http://fen.zhengqikj.top

Go:   resp.StatusCode
来源：http://trj.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://zdc.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://dsu.xuanzx.com

[L08] 并发请求多个地址
来源：http://tsq.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ree.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://vir.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rrc.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbh.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rja.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lgf.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://clg.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://axi.vqdsnc.cn

================================================================================
来源：http://bsy.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://yoq.xinyue.icu

================================================================================
来源：http://yxl.zdqjudy.top

[M01] 读取命令行参数
来源：http://asi.bjfxy.top

Py:   sys.argv[1:]
来源：http://jrj.316326.xyz

PHP:  $argv;  $argc;
来源：http://whj.bjfxy.top

JS:   process.argv.slice(2)
来源：http://txc.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://hbx.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://wpb.nwbrower.top

Go:   os.Args[1:]
来源：http://npg.uphjek.com

Ruby: ARGV
来源：http://nlo.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://fbh.yj20258888.top

[M02] 读取环境变量
来源：http://tcq.havefunace.top

Py:   os.environ.get("HOME")
来源：http://gro.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lbn.52xcode.cn

JS:   process.env.HOME
来源：http://dqu.yanxiufei.cn

TS:   process.env.HOME
来源：http://puj.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://qdr.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vct.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://wvi.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yhs.meibo888.top

[M03] 执行外部命令
来源：http://nug.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xzk.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zyx.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cod.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://upq.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://umm.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pnb.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://bzr.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://qlg.shuidangran.top

[M04] 获取当前工作目录
来源：http://gsc.zhiwuduotai.top

Py:   os.getcwd()
来源：http://hyp.c1oappe.top

PHP:  getcwd();
来源：http://zfu.nanxuanxn.top

JS:   process.cwd()
来源：http://vud.pengpengdd.cyou

TS:   process.cwd()
来源：http://xaa.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://wae.andypj.xyz

Go:   os.Getwd()
来源：http://uaq.cqqwz.cn

Ruby: Dir.pwd
来源：http://rud.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yjl.cdnleiting.top

[M05] 设置退出码
来源：http://hqd.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://sne.pengpengdd.cyou

PHP:  exit(1);
来源：http://wwy.feifeiyinyue.top

JS:   process.exit(1)
来源：http://zhu.gaohongyu789.top

TS:   process.exit(1)
来源：http://mwq.snrcjt.cn

Java: System.exit(1)
来源：http://fds.quarkkingdee.top

Go:   os.Exit(1)
来源：http://ibd.52xcode.cn

Ruby: exit 1
来源：http://tkj.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bil.havefunace.top

[M06] 向标准错误输出
来源：http://yio.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://xxq.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://gxh.jinghuilouyu.cn

JS:   console.error("err")
来源：http://vgg.zhongyouzk.top

TS:   console.error("err")
来源：http://yuw.jinqigufen.top

Java: System.err.println("err")
来源：http://pbi.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ktn.0kj1m.cn

Ruby: warn "err"
来源：http://jqe.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://itz.epnwcf.com

[M07] 判断是否为主入口
来源：http://nuh.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://cvc.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iuw.zhixingplan.top

JS:   require.main === module
来源：http://lkh.bbcook.cn

TS:   require.main === module
来源：http://kju.haohaochexian.top

Java: public static void main(String[] args)
来源：http://ofx.0kj1m.cn

Go:   func main()
来源：http://pky.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://weg.yuxming.cn

C#:   static void Main(string[] args)
来源：http://nae.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://bmk.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://nid.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://gfp.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://sgp.yuxming.cn

TS:   process.platform;  process.version
来源：http://rcd.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://prx.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oaf.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rfb.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://rmw.cqqwz.cn

================================================================================
来源：http://zap.yuxming.cn

N. 数据结构与算法
来源：http://ipx.zhixingplan.top

================================================================================
来源：http://ctj.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://trp.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://evz.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dhc.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ptl.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gih.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zwu.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://hwa.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bdp.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://ndj.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://wqd.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://bui.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mxm.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ccw.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bgb.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ops.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://awi.ivvv.top

Ruby: arr.sort
来源：http://zjd.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://hhn.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://qhe.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mcz.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://twp.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mte.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wmh.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vdp.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xde.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dic.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iip.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://tnj.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qsu.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uxa.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kyr.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qvy.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ttf.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zoi.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xjo.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cda.shzxlz.cn

[N05] 最大公约数
来源：http://dvp.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://gao.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tbf.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qll.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://esh.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gey.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mcm.gotoacloud.top

Ruby: a.gcd(b)
来源：http://uec.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xgg.epnwcf.com

[N06] 判断回文字符串
来源：http://xtg.tianlin.xyz

Py:   s == s[::-1]
来源：http://onm.mhx1999.top

PHP:  $s === strrev($s);
来源：http://pqf.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://vvt.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://epq.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://plb.shuidangran.top

Go:   // 双指针从两端比较
来源：http://hix.shuidangran.top


<!-- 参考信息 -->