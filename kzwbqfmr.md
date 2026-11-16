代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lio.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mwi.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tkd.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://mes.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iza.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://stj.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://avk.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bbu.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gnz.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vsg.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lkk.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hvv.zdbjq.cn

================================================================================
来源：http://jbv.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://jvd.sjlbkw.cn

================================================================================
来源：http://kkr.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://dao.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hvj.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ywj.yongpay.top

JS:   JSON.stringify(obj)
来源：http://dvj.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://kes.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bot.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://rcp.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rsc.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yyy.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://ksh.hnxiangtu.top

Py:   json.loads(s)
来源：http://igc.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hzs.meibo888.top

JS:   JSON.parse(s)
来源：http://bxz.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://fmv.nanxuanxn.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hfp.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://npf.aizwys.cn

Ruby: JSON.parse(s)
来源：http://jin.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lxx.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://tbt.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vex.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mpu.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nwj.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://lnj.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hhv.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iiw.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://aye.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mbz.ivvv.top

[K04] 读取 JSON 文件
来源：http://rbg.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ifd.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wkz.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lce.chenjidiqi.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vwi.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mtz.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kiy.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tah.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yij.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://ava.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://nzs.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://vxc.ybcxt.top

JS:   structuredClone(obj)
来源：http://sqs.yj20258.top

TS:   structuredClone(obj)
来源：http://ums.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wgz.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nsz.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dob.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://dra.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://lsx.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ekz.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yny.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://okz.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ewk.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wag.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tfi.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gll.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qqf.sxryk.cn

[K07] 进制转换
来源：http://sep.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ghg.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wix.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://len.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://paq.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wfr.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jnl.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://elj.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pbn.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://gxk.ivvv.top

Py:   pickle.dumps(obj)
来源：http://rit.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sqw.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://vtn.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://tse.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ncp.zycfv.cn

Go:   encoding/gob
来源：http://rvw.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://yqw.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hjw.xuanzx.com

================================================================================
来源：http://qtc.yvedp.cn

L. 网络请求
来源：http://izx.snrcjt.cn

================================================================================
来源：http://qnv.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://yqh.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dnz.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qjv.zhongyouzk.top

JS:   await fetch(url)
来源：http://hmr.xuetiantiany.cn

TS:   await fetch(url)
来源：http://hzc.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lob.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://raj.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jcy.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nbt.mhx1999.top

[L02] 发送 POST JSON
来源：http://wvu.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ebb.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mbl.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://auj.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fta.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yfv.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ucs.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cul.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lfm.sxryk.cn

[L03] 设置自定义请求头
来源：http://xtf.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zwb.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mks.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qzr.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nic.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rin.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bsl.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://red.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sfx.yuxming.cn

[L04] 设置超时
来源：http://rja.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://yke.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bvk.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tga.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vuo.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://czk.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nfr.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kjo.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fhc.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://vwx.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bpp.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tpt.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vnz.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jsm.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cfk.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://koc.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xui.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rgg.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://xge.wangshuangyany.cn

Py:   resp.json()
来源：http://bbg.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://drg.shuidangran.top

JS:   await resp.json()
来源：http://lhd.redwolf501.top

TS:   await resp.json()
来源：http://arw.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sbe.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://czj.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://rcd.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tyh.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://asg.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://phv.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hzn.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://ovs.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://wxs.jiagoushi.top

Java: resp.statusCode()
来源：http://nav.sjlbkw.cn

Go:   resp.StatusCode
来源：http://cwb.xuanzx.com

Ruby: resp.code.to_i
来源：http://qaf.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://yam.zdqjudy.top

[L08] 并发请求多个地址
来源：http://guc.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kza.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://aiv.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://klp.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ntl.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ycx.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ljt.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dkp.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fiy.vqdsnc.cn

================================================================================
来源：http://aoz.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://nzx.yj202588.top

================================================================================
来源：http://aqa.andypj.xyz

[M01] 读取命令行参数
来源：http://wct.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://tmx.uphjek.com

PHP:  $argv;  $argc;
来源：http://yrm.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://zrj.ybcxt.top

TS:   process.argv.slice(2)
来源：http://vqi.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://cjj.hywenlv.cn

Go:   os.Args[1:]
来源：http://qwv.chenzaomai.com

Ruby: ARGV
来源：http://vxp.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://sju.nanxuanxn.top

[M02] 读取环境变量
来源：http://ijk.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://kva.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yji.hywenlv.cn

JS:   process.env.HOME
来源：http://hvc.mhx1999.top

TS:   process.env.HOME
来源：http://wav.hnqzz.top

Java: System.getenv("HOME")
来源：http://eec.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eff.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://kot.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uzh.sufxvd.cn

[M03] 执行外部命令
来源：http://ohi.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gfq.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xnw.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jqy.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ihn.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://msa.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://gnw.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jqa.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://vpk.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://eho.bjfxy.top

Py:   os.getcwd()
来源：http://hdf.jianghu66.top

PHP:  getcwd();
来源：http://ejr.uphjek.com

JS:   process.cwd()
来源：http://ger.yj20258888.top

TS:   process.cwd()
来源：http://edg.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://cjs.feifeiyinyue.top

Go:   os.Getwd()
来源：http://xyu.hysaishi.cn

Ruby: Dir.pwd
来源：http://cjy.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://mdd.dianchejie.cn

[M05] 设置退出码
来源：http://jhp.yongpay.top

Py:   sys.exit(1)
来源：http://oqo.yanxiufei.cn

PHP:  exit(1);
来源：http://dwh.cdnleiting.top

JS:   process.exit(1)
来源：http://fkt.xuetiantiany.cn

TS:   process.exit(1)
来源：http://ezp.ehwqpu.com

Java: System.exit(1)
来源：http://die.pycfn.com

Go:   os.Exit(1)
来源：http://nrc.tian-w.cn

Ruby: exit 1
来源：http://dog.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://feq.ydjk.org.cn

[M06] 向标准错误输出
来源：http://qbb.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://ecw.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hrj.jiagoushi.top

JS:   console.error("err")
来源：http://cnz.jiagoushi.top

TS:   console.error("err")
来源：http://dqc.c1oappe.top

Java: System.err.println("err")
来源：http://mlm.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cax.yangfankeji.com

Ruby: warn "err"
来源：http://off.jqgfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://rwu.yuxming.cn

[M07] 判断是否为主入口
来源：http://wbf.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://sab.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wja.hfpthk.cn

JS:   require.main === module
来源：http://xeq.dashuyun.cn

TS:   require.main === module
来源：http://xwj.jiagoushi.top

Java: public static void main(String[] args)
来源：http://tzt.jyoumei.cn

Go:   func main()
来源：http://gky.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pms.andypj.xyz

C#:   static void Main(string[] args)
来源：http://azt.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://xpu.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://ihx.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://jmp.yvedp.cn

JS:   process.platform;  process.version
来源：http://qko.aizwys.cn

TS:   process.platform;  process.version
来源：http://hzm.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xyl.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lqp.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oao.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fcw.chenjidiqi.icu

================================================================================
来源：http://lrm.sufxvd.cn

N. 数据结构与算法
来源：http://zvg.nwbrower.top

================================================================================
来源：http://wrj.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://jjw.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://vze.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iip.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://skl.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fvs.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ieg.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://oaj.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ruo.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://hmn.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://rtu.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://lhu.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cnx.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yrj.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hfp.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ocm.nwbrower.top

Go:   slices.Sort(arr)
来源：http://cin.wangshuangyany.cn

Ruby: arr.sort
来源：http://qws.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vtr.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://cgn.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qsq.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://xoj.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wsw.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qyh.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gqg.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ghm.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://efy.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://nvz.yonumen.top

[N04] 斐波那契数列
来源：http://efh.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://twt.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wiv.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vbn.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iaa.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tbl.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://twz.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tnq.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://trl.hnxiangtu.top

[N05] 最大公约数
来源：http://rco.havefunace.top

Py:   math.gcd(a, b)
来源：http://zia.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://znp.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jtc.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ynd.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zta.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lgy.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://qhl.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://szr.gaohongyu789.top

[N06] 判断回文字符串
来源：http://auf.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://nrb.cheryme.top

PHP:  $s === strrev($s);
来源：http://zvk.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://dtb.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://nsq.yuanzhike.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fye.zycfv.cn

Go:   // 双指针从两端比较
来源：http://vrg.birdmap.top

Ruby: s == s.reverse
来源：http://lju.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kfi.havefunace.top

[N07] 两数之和（返回下标）
来源：http://twl.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iau.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tjt.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ttd.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://ppr.epnwcf.com

Java: // 手写 HashMap
来源：http://lcq.sxryk.cn


<!-- 参考信息 -->