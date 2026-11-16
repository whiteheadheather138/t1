代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sqw.tanke756.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bjm.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zlf.daria6918.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wur.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lor.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://abr.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wjm.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://kwj.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://skk.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uah.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jef.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kpm.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pxu.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sou.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dqv.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eus.fzhhl.top

================================================================================
来源：http://yng.guowangkeji.top

K. JSON 与序列化
来源：http://xik.jqgfzy.top

================================================================================
来源：http://jwx.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://qto.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pyc.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rmt.meibo888.top

JS:   JSON.stringify(obj)
来源：http://zul.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://wwl.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dtj.tian-w.cn

Go:   json.Marshal(obj)
来源：http://lkh.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://tba.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://yld.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://rce.hcnkem.com

Py:   json.loads(s)
来源：http://frc.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nov.yj202588.top

JS:   JSON.parse(s)
来源：http://ina.yj202588.top

TS:   JSON.parse(s)
来源：http://oxd.svipenyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gri.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://dbp.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://hty.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fse.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://qol.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gwd.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aln.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ion.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nfd.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wvz.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zcg.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hlo.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qgj.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://unk.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ror.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kew.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pqf.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qep.hesvh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nhm.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aeo.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xse.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wrf.cashguo.top

[K05] 深拷贝对象
来源：http://lav.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://vgz.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://tcj.9152youxi.cn

JS:   structuredClone(obj)
来源：http://llv.zhixingplan.top

TS:   structuredClone(obj)
来源：http://mmj.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://gbv.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ctw.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cgh.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rvi.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://mzn.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gbj.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://opd.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pzv.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://goq.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rdd.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fqf.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ewi.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lec.yuanzhike.top

[K07] 进制转换
来源：http://wdp.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hkh.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://slf.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://spp.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wml.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gnz.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jgr.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sgw.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://frl.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://tyi.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://qex.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iik.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://wjd.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://gpd.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fex.ydjk.org.cn

Go:   encoding/gob
来源：http://uho.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://awp.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://acr.aizwys.cn

================================================================================
来源：http://blo.dashuyun.cn

L. 网络请求
来源：http://cpl.guannengcc.top

================================================================================
来源：http://eji.andypj.xyz

[L01] 发送 GET 请求
来源：http://kca.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://egh.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vpb.sjlbkw.cn

JS:   await fetch(url)
来源：http://ivl.zhongyouzk.top

TS:   await fetch(url)
来源：http://jyb.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mxp.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://val.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gox.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lkq.tian-w.cn

[L02] 发送 POST JSON
来源：http://jwf.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ulp.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bee.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://owm.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://alw.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ahr.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xhh.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bdv.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jjn.yfazqb.com

[L03] 设置自定义请求头
来源：http://zih.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ntw.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ege.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uuy.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsg.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vxi.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iwv.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bvs.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xyh.jinghuilouyu.cn

[L04] 设置超时
来源：http://wxm.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://ncw.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kqa.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vju.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xrq.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lhw.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wbw.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://upm.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gqb.wangdashe.top

[L05] 上传文件（multipart）
来源：http://uem.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cej.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sdw.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pfv.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://upj.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yxz.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eei.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://smo.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nrn.fehbvm.com

[L06] 解析响应为 JSON
来源：http://yvd.wangshuangyany.cn

Py:   resp.json()
来源：http://woo.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://irl.dianchejie.cn

JS:   await resp.json()
来源：http://oax.yj20258.top

TS:   await resp.json()
来源：http://fiw.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bvq.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mwu.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://cmn.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jpu.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://hje.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://auc.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wex.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://vzw.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://nxr.hammf.cn

Java: resp.statusCode()
来源：http://ocq.vehdjk.com

Go:   resp.StatusCode
来源：http://ymk.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://byb.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://ckn.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://aiy.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fvx.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://uno.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ubf.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://msw.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uoi.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://anq.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mqn.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gfo.xinyue.icu

================================================================================
来源：http://wdu.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://iwv.zycfv.cn

================================================================================
来源：http://sgd.9152youxi.cn

[M01] 读取命令行参数
来源：http://hfr.52xcode.cn

Py:   sys.argv[1:]
来源：http://ghi.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://lxi.hesvh.cn

JS:   process.argv.slice(2)
来源：http://ygq.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://lyu.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://gbq.guannengcc.top

Go:   os.Args[1:]
来源：http://ogx.epnwcf.com

Ruby: ARGV
来源：http://qlr.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://ucy.cucudq.cn

[M02] 读取环境变量
来源：http://gjm.316326.xyz

Py:   os.environ.get("HOME")
来源：http://acq.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kkx.sxryk.cn

JS:   process.env.HOME
来源：http://mko.hammf.cn

TS:   process.env.HOME
来源：http://jhs.cheryme.top

Java: System.getenv("HOME")
来源：http://yas.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gxm.cheryme.top

Ruby: ENV["HOME"]
来源：http://mlo.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ful.feifeiyinyue.top

[M03] 执行外部命令
来源：http://pge.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qsl.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sey.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rol.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://hgh.cdnleiting.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nuq.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://atu.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://llg.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://rbe.tanke756.top

[M04] 获取当前工作目录
来源：http://xjo.9152youxi.cn

Py:   os.getcwd()
来源：http://yzn.cashguo.top

PHP:  getcwd();
来源：http://dbz.ydjk.org.cn

JS:   process.cwd()
来源：http://eea.hnqzz.top

TS:   process.cwd()
来源：http://esa.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://vew.chenzaomai.com

Go:   os.Getwd()
来源：http://mmu.hysaishi.cn

Ruby: Dir.pwd
来源：http://twb.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://jro.hammf.cn

[M05] 设置退出码
来源：http://erf.ppjwa.cn

Py:   sys.exit(1)
来源：http://lzg.cheryme.top

PHP:  exit(1);
来源：http://lcf.pycfn.com

JS:   process.exit(1)
来源：http://vau.daria6918.cn

TS:   process.exit(1)
来源：http://fsa.gaohongyu789.top

Java: System.exit(1)
来源：http://fmc.ydzc1.top

Go:   os.Exit(1)
来源：http://vdl.vqdsnc.cn

Ruby: exit 1
来源：http://sns.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://khy.aizwys.cn

[M06] 向标准错误输出
来源：http://gji.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://odd.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nch.nanxuanxn.top

JS:   console.error("err")
来源：http://mut.cdnleiting.top

TS:   console.error("err")
来源：http://rdw.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://uiw.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tnf.fktsv.cn

Ruby: warn "err"
来源：http://ufl.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://ral.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://hbs.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://kct.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xhg.zhengqikj.top

JS:   require.main === module
来源：http://vjx.cheryme.top

TS:   require.main === module
来源：http://wpl.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://cuj.andypj.xyz

Go:   func main()
来源：http://hex.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fqy.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://ioq.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://gul.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://dgq.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://dhu.zdqjudy.top

JS:   process.platform;  process.version
来源：http://gwt.c1oappe.top

TS:   process.platform;  process.version
来源：http://coj.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://irw.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bsw.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ayu.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://eke.yanxiufei.cn

================================================================================
来源：http://tef.fanxiaobao.xyz

N. 数据结构与算法
来源：http://grx.cucudq.cn

================================================================================
来源：http://zcz.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://ubs.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://trx.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pfs.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mye.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://acw.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yfd.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://ioe.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lsp.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fqu.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://vuc.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://tkx.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nmx.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mvr.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jyh.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nlg.cashguo.top

Go:   slices.Sort(arr)
来源：http://oui.gogol.net.cn

Ruby: arr.sort
来源：http://rse.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://hrz.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://bjz.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jdg.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://pgl.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://paa.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zxo.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ynp.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iok.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eqh.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://mwq.shanyushiyangkeji.top

[N04] 斐波那契数列
来源：http://wpi.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lwk.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ift.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://amw.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://apv.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ptj.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vch.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://con.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://swp.fktsv.cn

[N05] 最大公约数
来源：http://qhj.xuanzx.com

Py:   math.gcd(a, b)
来源：http://mhh.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ixv.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ypa.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lye.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ujn.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ucf.chenlongwang.top

Ruby: a.gcd(b)
来源：http://vod.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xdy.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://zms.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://fsi.sweek.top

PHP:  $s === strrev($s);
来源：http://gkf.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://who.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://pis.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vyg.hesvh.cn

Go:   // 双指针从两端比较
来源：http://oty.yuxming.cn

Ruby: s == s.reverse
来源：http://nku.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wel.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://bxj.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nyh.mhx1999.top


<!-- 参考信息 -->