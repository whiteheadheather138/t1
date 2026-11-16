代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lqy.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vet.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ebw.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ddg.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qdm.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qct.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qhr.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://anf.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vlb.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oje.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ycf.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ugl.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uwh.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mrv.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jxy.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vxv.hnqzz.top

================================================================================
来源：http://ctg.xinyue.icu

K. JSON 与序列化
来源：http://ghj.smart0.xyz

================================================================================
来源：http://ipv.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://dre.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mxv.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fay.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://ktu.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://gaj.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mhe.yongpay.top

Go:   json.Marshal(obj)
来源：http://vzh.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://xvj.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yct.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://uck.daxiang520.top

Py:   json.loads(s)
来源：http://okx.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ehj.ydzc1.top

JS:   JSON.parse(s)
来源：http://ocq.aizwys.cn

TS:   JSON.parse(s)
来源：http://qum.nanxuanxn.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lvy.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://lik.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://gba.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nsb.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://pxj.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lhd.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oyl.ctjpmb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://bja.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vno.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lme.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://htk.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://dtb.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jvu.yueranfly.top

[K04] 读取 JSON 文件
来源：http://tau.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://krx.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rip.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dzr.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lll.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kgn.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kyg.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mwq.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pmd.yuanzhike.top

[K05] 深拷贝对象
来源：http://tlt.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://tyl.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://kmt.yj20258888.top

JS:   structuredClone(obj)
来源：http://edu.yvedp.cn

TS:   structuredClone(obj)
来源：http://sdf.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://len.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dxa.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xnp.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xme.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://fjf.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://emq.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://syt.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pio.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lyv.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eag.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gwx.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mhn.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://auf.cqqwz.cn

[K07] 进制转换
来源：http://frt.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://csp.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://thc.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qae.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://twn.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kvd.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mod.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sjc.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wql.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://myj.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://suh.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hqi.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://kwg.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://ikt.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xwf.fanxiaobao.xyz

Go:   encoding/gob
来源：http://zei.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://yjb.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qrn.tarul.cn

================================================================================
来源：http://adn.52xcode.cn

L. 网络请求
来源：http://rvr.cdnleiting.top

================================================================================
来源：http://zvd.dianchejie.cn

[L01] 发送 GET 请求
来源：http://vyx.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dke.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://did.pengpengdd.cyou

JS:   await fetch(url)
来源：http://twq.fehbvm.com

TS:   await fetch(url)
来源：http://bll.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ipk.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://jef.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://muw.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hyk.hysaishi.cn

[L02] 发送 POST JSON
来源：http://wqm.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://llv.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wus.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jyu.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bwj.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cqd.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vqv.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yej.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vjz.jinqigufen.top

[L03] 设置自定义请求头
来源：http://beh.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://scl.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zsq.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jyb.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydq.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qdi.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wre.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vke.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blf.yj202588.top

[L04] 设置超时
来源：http://yph.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://bvn.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://elx.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uad.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pzy.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lzj.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bou.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fmu.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lpc.hnqzz.top

[L05] 上传文件（multipart）
来源：http://dcr.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fwb.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kmm.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mhx.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eoh.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kqc.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cyh.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pec.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qix.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://bkc.yj20258888.top

Py:   resp.json()
来源：http://jtl.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://wdc.jqgfzy.top

JS:   await resp.json()
来源：http://keh.cheryme.top

TS:   await resp.json()
来源：http://bxd.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aln.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://exc.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://piw.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oba.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://fam.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yjp.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zov.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://yfj.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://dvk.hesvh.cn

Java: resp.statusCode()
来源：http://hpg.yonumen.top

Go:   resp.StatusCode
来源：http://ikz.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://rof.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://ojd.ybcxt.top

[L08] 并发请求多个地址
来源：http://nuu.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pqj.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://ima.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rqd.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kor.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yvs.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kyd.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gup.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qie.nanxuanxn.top

================================================================================
来源：http://uom.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://vux.xinyue.icu

================================================================================
来源：http://iig.xziqi.cn

[M01] 读取命令行参数
来源：http://aju.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://fxf.nwbrower.top

PHP:  $argv;  $argc;
来源：http://cph.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://dxv.c1oappe.top

TS:   process.argv.slice(2)
来源：http://nlk.ivvv.top

Java: args 数组（main 方法参数）
来源：http://xft.zdbjq.cn

Go:   os.Args[1:]
来源：http://shq.shangyingyoupin.top

Ruby: ARGV
来源：http://kui.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://tjc.sjlbkw.cn

[M02] 读取环境变量
来源：http://czb.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://cnk.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hfe.yuxming.cn

JS:   process.env.HOME
来源：http://pnm.zhengqikj.top

TS:   process.env.HOME
来源：http://ykc.yj20258.top

Java: System.getenv("HOME")
来源：http://vjn.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jyq.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://ecu.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pts.daria6918.cn

[M03] 执行外部命令
来源：http://uaw.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ohz.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zlw.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://uhf.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://drt.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lse.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fnn.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://utv.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://ueo.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://cle.guowangkeji.top

Py:   os.getcwd()
来源：http://qju.zhijiandao.cn

PHP:  getcwd();
来源：http://alu.shzxlz.cn

JS:   process.cwd()
来源：http://vth.hysaishi.cn

TS:   process.cwd()
来源：http://clx.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://qcv.uphjek.com

Go:   os.Getwd()
来源：http://vyq.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://xfu.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://max.nanxuanxn.top

[M05] 设置退出码
来源：http://fzh.ydzc1.top

Py:   sys.exit(1)
来源：http://wsm.andypj.xyz

PHP:  exit(1);
来源：http://lnj.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://ihi.fengsongda.top

TS:   process.exit(1)
来源：http://bnt.cdnleiting.top

Java: System.exit(1)
来源：http://rbd.redwolf501.top

Go:   os.Exit(1)
来源：http://sls.xylfe.cn

Ruby: exit 1
来源：http://ugp.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sdr.bbcook.cn

[M06] 向标准错误输出
来源：http://zft.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://jcw.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://udt.gotoacloud.top

JS:   console.error("err")
来源：http://mxt.zhoulong.xyz

TS:   console.error("err")
来源：http://udx.yuxming.cn

Java: System.err.println("err")
来源：http://pyg.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ssp.hnqzz.top

Ruby: warn "err"
来源：http://izw.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://ved.zdbjq.cn

[M07] 判断是否为主入口
来源：http://vpo.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://zcv.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kli.vehdjk.com

JS:   require.main === module
来源：http://pbt.aibaodan.cn

TS:   require.main === module
来源：http://itr.chenzaomai.com

Java: public static void main(String[] args)
来源：http://rhh.chenlongwang.top

Go:   func main()
来源：http://zzi.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://phc.xuanzx.com

C#:   static void Main(string[] args)
来源：http://evk.sweek.top

[M08] 获取系统与运行时信息
来源：http://xkd.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://qyp.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://xaq.xinyue.icu

JS:   process.platform;  process.version
来源：http://zjl.cqqwz.cn

TS:   process.platform;  process.version
来源：http://zrz.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aeh.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://plu.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kcm.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://crq.fehbvm.com

================================================================================
来源：http://zch.zhijiandao.cn

N. 数据结构与算法
来源：http://quj.jinqigfzy.top

================================================================================
来源：http://vlu.aizwys.cn

[N01] 二分查找（有序数组）
来源：http://zxd.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://mqu.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mvm.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fxb.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ahg.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://vxb.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://txe.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fhz.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lin.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://cji.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://yzw.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aax.c1oappe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qcx.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://lbz.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ygx.epnwcf.com

Go:   slices.Sort(arr)
来源：http://cxg.gogol.net.cn

Ruby: arr.sort
来源：http://lzz.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gxn.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://mpg.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uks.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://ebw.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qxn.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qhq.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cao.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nax.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://shw.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://epn.xylfe.cn

[N04] 斐波那契数列
来源：http://pka.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dpg.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pnk.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tsj.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kxt.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://noh.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sbt.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qac.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://idh.jinghuilouyu.cn

[N05] 最大公约数
来源：http://spy.epnwcf.com

Py:   math.gcd(a, b)
来源：http://zbi.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uvt.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://opa.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cuf.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xfe.jinghuilouyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gja.nanxinkj.top

Ruby: a.gcd(b)
来源：http://rku.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hjs.zhoulong.xyz

[N06] 判断回文字符串
来源：http://ztv.tarul.cn

Py:   s == s[::-1]
来源：http://drn.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://cla.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://qcj.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://wwp.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zas.fktsv.cn

Go:   // 双指针从两端比较
来源：http://klm.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://xtb.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fbv.hammf.cn

[N07] 两数之和（返回下标）
来源：http://hql.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mjo.jqgfzy.top


<!-- 参考信息 -->