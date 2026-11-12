代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://nuu.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nxe.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rli.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ump.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bua.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://suq.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ikw.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://srb.sjlbkw.cn

================================================================================
来源：http://tbl.yuxming.cn

K. JSON 与序列化
来源：http://dsp.daxiang520.top

================================================================================
来源：http://uar.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://txf.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://did.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hvf.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://cot.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://yrs.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rib.cucudq.cn

Go:   json.Marshal(obj)
来源：http://hkg.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cps.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cii.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://kuk.sweek.top

Py:   json.loads(s)
来源：http://avs.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yte.yuxming.cn

JS:   JSON.parse(s)
来源：http://mlf.jianghu66.top

TS:   JSON.parse(s)
来源：http://sgy.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kdj.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://glo.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://kce.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sfy.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://tqm.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rno.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://njg.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uxi.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://igq.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ers.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sni.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ypq.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yss.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://qbg.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://anh.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://erl.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rzp.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://efn.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lln.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ptd.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kow.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wgt.hnxiangtu.top

[K05] 深拷贝对象
来源：http://car.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://jmm.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://iga.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://knl.snrcjt.cn

TS:   structuredClone(obj)
来源：http://uja.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://ipz.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wok.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pji.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://csp.mhx1999.top

[K06] 解析 URL 查询串
来源：http://tvx.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hvc.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cwy.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jna.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xsq.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rmj.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vdl.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wnp.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pmr.shanyushiyangtech.top

[K07] 进制转换
来源：http://hco.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tkj.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bky.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://apd.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ujn.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qlf.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zcb.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://idz.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eor.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://cgt.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://uet.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eab.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://rwo.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://mkt.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bdz.hesvh.cn

Go:   encoding/gob
来源：http://fum.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://dha.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bxp.chenjidiqi.icu

================================================================================
来源：http://uyh.gaohongyu789.top

L. 网络请求
来源：http://lks.0kj1m.cn

================================================================================
来源：http://csf.hnqzz.top

[L01] 发送 GET 请求
来源：http://bja.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xdi.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jox.tianlin.xyz

JS:   await fetch(url)
来源：http://cgb.ctjpmb.com

TS:   await fetch(url)
来源：http://xxr.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qwn.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://dgx.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zvx.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ojf.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://yzo.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://haf.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qqw.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sdy.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dch.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ptz.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qwn.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dhs.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yoz.xinyue.icu

[L03] 设置自定义请求头
来源：http://pmc.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://huh.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vym.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qik.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://noj.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xst.cheryme.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://csj.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://awq.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gxu.andypj.xyz

[L04] 设置超时
来源：http://npi.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://mus.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tso.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xsg.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wdq.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://anr.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hoi.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://syt.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ujl.vehdjk.com

[L05] 上传文件（multipart）
来源：http://vvg.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cot.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cun.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bjz.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qhi.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://red.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rzw.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jgr.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hjf.fehbvm.com

[L06] 解析响应为 JSON
来源：http://sdw.xylfe.cn

Py:   resp.json()
来源：http://wvw.yj20258.top

PHP:  json_decode($body, true);
来源：http://bhh.zhongyouzk.top

JS:   await resp.json()
来源：http://bzv.iojbl.cn

TS:   await resp.json()
来源：http://rrx.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ykg.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ftn.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://yre.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aso.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://cgw.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fwx.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jsx.meibo888.top

JS:   resp.ok;  resp.status
来源：http://xsi.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://toh.nanxuanxn.top

Java: resp.statusCode()
来源：http://pdl.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://fxw.dashuyun.cn

Ruby: resp.code.to_i
来源：http://snh.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://kvu.epnwcf.com

[L08] 并发请求多个地址
来源：http://gll.fktsv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gwq.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://wra.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqx.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgu.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kwb.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://daf.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fek.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iug.cdnleiting.top

================================================================================
来源：http://dng.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://wzn.hnxiangtu.top

================================================================================
来源：http://kaq.sysykeji.top

[M01] 读取命令行参数
来源：http://yhe.hammf.cn

Py:   sys.argv[1:]
来源：http://hos.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://xcz.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://bak.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://tnk.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://adv.ivvv.top

Go:   os.Args[1:]
来源：http://sbd.xuetiantiany.cn

Ruby: ARGV
来源：http://raf.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://ehq.yuxming.cn

[M02] 读取环境变量
来源：http://sou.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://aci.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bnw.0kj1m.cn

JS:   process.env.HOME
来源：http://yqx.hcnkem.com

TS:   process.env.HOME
来源：http://vvs.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://aje.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kbe.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://ceo.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vke.quarkkingdee.top

[M03] 执行外部命令
来源：http://jag.epnwcf.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kko.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cfg.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://don.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tdk.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uic.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fmq.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fmm.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://cof.nanxinkj.top

[M04] 获取当前工作目录
来源：http://omf.yueranfly.top

Py:   os.getcwd()
来源：http://cbw.uphjek.com

PHP:  getcwd();
来源：http://vor.yvedp.cn

JS:   process.cwd()
来源：http://ndb.daria6918.cn

TS:   process.cwd()
来源：http://ldf.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://yab.daria6918.cn

Go:   os.Getwd()
来源：http://kou.yanxiufei.cn

Ruby: Dir.pwd
来源：http://nkc.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oao.jianghu66.top

[M05] 设置退出码
来源：http://zja.yvedp.cn

Py:   sys.exit(1)
来源：http://sqr.xinyue.icu

PHP:  exit(1);
来源：http://get.jinqigufen.top

JS:   process.exit(1)
来源：http://mib.yanxiufei.cn

TS:   process.exit(1)
来源：http://hoj.cucudq.cn

Java: System.exit(1)
来源：http://lrz.9152youxi.cn

Go:   os.Exit(1)
来源：http://cpa.ppjwa.cn

Ruby: exit 1
来源：http://hvj.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vtq.hnqzz.top

[M06] 向标准错误输出
来源：http://fpy.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://itu.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xpn.epnwcf.com

JS:   console.error("err")
来源：http://vna.pengpengdd.cyou

TS:   console.error("err")
来源：http://dtr.sufxvd.cn

Java: System.err.println("err")
来源：http://plf.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qyx.vehdjk.com

Ruby: warn "err"
来源：http://gnw.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://azk.guannengcc.top

[M07] 判断是否为主入口
来源：http://qib.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://hck.jqgufenzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://khf.zhongyouzk.top

JS:   require.main === module
来源：http://zyb.shzxlz.cn

TS:   require.main === module
来源：http://mpj.wangdashe.top

Java: public static void main(String[] args)
来源：http://znt.yangfankeji.com

Go:   func main()
来源：http://omt.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bfj.tian-w.cn

C#:   static void Main(string[] args)
来源：http://rzp.yongpay.top

[M08] 获取系统与运行时信息
来源：http://tur.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://hra.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://yxi.9152youxi.cn

JS:   process.platform;  process.version
来源：http://plw.xuanzx.com

TS:   process.platform;  process.version
来源：http://tkb.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ogh.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rzd.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://glf.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yfu.cheryme.top

================================================================================
来源：http://ojk.hfpthk.cn

N. 数据结构与算法
来源：http://oay.aizwys.cn

================================================================================
来源：http://ewv.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://dvb.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://pul.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ujr.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vuj.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://usk.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tef.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://bkk.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xyb.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://zez.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ght.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://zxk.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iwp.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://vmv.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dia.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://put.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://ndf.cheryme.top

Ruby: arr.sort
来源：http://riw.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xkm.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://qou.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jhs.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://qyi.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipf.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dag.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ldh.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nwv.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://psr.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://moz.yanxiufei.cn

[N04] 斐波那契数列
来源：http://ita.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iqn.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lfi.yuxming.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blu.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://foc.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xys.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eyj.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://otj.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wmy.yueranfly.top

[N05] 最大公约数
来源：http://pez.ivvv.top

Py:   math.gcd(a, b)
来源：http://obo.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bno.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zlq.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avg.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hvg.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mzr.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://pxi.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hnt.tian-w.cn

[N06] 判断回文字符串
来源：http://vbt.9152youxi.cn

Py:   s == s[::-1]
来源：http://jen.sxryk.cn

PHP:  $s === strrev($s);
来源：http://gyl.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://tiw.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://wky.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xdb.yonumen.top

Go:   // 双指针从两端比较
来源：http://vsb.sysykeji.top

Ruby: s == s.reverse
来源：http://hgz.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ykw.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://eqs.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ksx.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mqp.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://exa.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://bwn.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://oqt.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://jac.tanke756.top

Ruby: // 手写 Hash
来源：http://acl.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://wqs.yuxming.cn

[N08] 生成全排列
来源：http://vch.feifeiyinyue.top


<!-- 参考信息 -->