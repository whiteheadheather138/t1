代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://wmv.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://knf.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hdh.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mar.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kis.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brt.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hsf.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yyp.yueranfly.top

================================================================================
来源：http://smn.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://xty.9152youxi.cn

================================================================================
来源：http://zum.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://ukf.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://etg.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ngp.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://jcj.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://fzl.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://esb.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://mvf.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://qak.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://znk.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://xyw.dashuyun.cn

Py:   json.loads(s)
来源：http://ejn.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ktd.tarul.cn

JS:   JSON.parse(s)
来源：http://xmn.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://nmh.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qjr.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://qcv.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://fto.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wpo.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://mzu.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sqv.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ywj.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oct.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uja.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jfx.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ecu.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://vcw.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jiv.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://ghs.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://anh.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yaa.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hhv.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://avc.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wak.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nbn.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mrg.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vnj.ppjwa.cn

[K05] 深拷贝对象
来源：http://cps.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://wxq.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://yqg.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://bze.zhixingplan.top

TS:   structuredClone(obj)
来源：http://jqg.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fas.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ifn.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mpq.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gqp.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://gia.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wxa.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rkk.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wph.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ozk.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yrr.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vny.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ezj.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jtn.dashuyun.cn

[K07] 进制转换
来源：http://oyq.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bkx.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lkn.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dib.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://azs.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tto.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ggc.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xpr.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xyc.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://ufc.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://glc.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rpc.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://xoo.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://pbm.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://swk.zhijiandao.cn

Go:   encoding/gob
来源：http://lxj.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://ppc.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wes.fzhhl.top

================================================================================
来源：http://mfh.zhongyouzk.top

L. 网络请求
来源：http://bxd.fehbvm.com

================================================================================
来源：http://ire.0kj1m.cn

[L01] 发送 GET 请求
来源：http://tyl.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hcg.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iuo.xuanzx.com

JS:   await fetch(url)
来源：http://xgi.zhengqikj.top

TS:   await fetch(url)
来源：http://zzp.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eem.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://ldx.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qja.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zpo.yj20258888.top

[L02] 发送 POST JSON
来源：http://meq.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://caj.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ami.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpe.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bwz.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ori.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lyf.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mij.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mex.cheryme.top

[L03] 设置自定义请求头
来源：http://ujn.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nqp.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ksc.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ott.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wmq.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://klv.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dux.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ywu.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vrc.aizwys.cn

[L04] 设置超时
来源：http://zbn.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://wts.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xxs.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ydp.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ahr.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hpk.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zqh.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://haa.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bmr.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://gtn.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aaw.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wlz.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mzv.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://njh.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gkc.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pys.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yvv.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://npf.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://kwe.snrcjt.cn

Py:   resp.json()
来源：http://yoe.tian-w.cn

PHP:  json_decode($body, true);
来源：http://bbz.fanxiaobao.xyz

JS:   await resp.json()
来源：http://mcm.hammf.cn

TS:   await resp.json()
来源：http://roa.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ain.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bjq.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://mrk.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uvg.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://fte.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nat.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://itf.316326.xyz

JS:   resp.ok;  resp.status
来源：http://kbk.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://exi.jqgufenzy.top

Java: resp.statusCode()
来源：http://uyv.jlsjyb.cn

Go:   resp.StatusCode
来源：http://fuc.9152youxi.cn

Ruby: resp.code.to_i
来源：http://dnk.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://uku.redwolf501.top

[L08] 并发请求多个地址
来源：http://bbs.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uxh.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://ruw.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hrn.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwr.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dbr.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jxn.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://har.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uur.tarul.cn

================================================================================
来源：http://hpt.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://vqj.hesvh.cn

================================================================================
来源：http://omo.zhengqikj.top

[M01] 读取命令行参数
来源：http://yhv.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://adx.sysykeji.top

PHP:  $argv;  $argc;
来源：http://xcg.vehdjk.com

JS:   process.argv.slice(2)
来源：http://npo.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://qkw.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://utk.daxiang520.top

Go:   os.Args[1:]
来源：http://uku.daria6918.cn

Ruby: ARGV
来源：http://oua.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://bxj.uphjek.com

[M02] 读取环境变量
来源：http://eqz.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://nsr.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qxd.epnwcf.com

JS:   process.env.HOME
来源：http://jhg.xinyue.icu

TS:   process.env.HOME
来源：http://lpq.aizwys.cn

Java: System.getenv("HOME")
来源：http://wvy.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qpx.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://avb.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://keo.yuanzhike.top

[M03] 执行外部命令
来源：http://pfm.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bgg.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ovi.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://kxg.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://rhm.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://its.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://hvo.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://roy.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://pvk.yongpay.top

[M04] 获取当前工作目录
来源：http://lwk.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://rdz.nanxuanxn.top

PHP:  getcwd();
来源：http://pjy.kuanghao11.cn

JS:   process.cwd()
来源：http://pcm.yangfankeji.com

TS:   process.cwd()
来源：http://vnl.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://elx.andypj.xyz

Go:   os.Getwd()
来源：http://ree.jyoumei.cn

Ruby: Dir.pwd
来源：http://doo.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://xhe.bbcook.cn

[M05] 设置退出码
来源：http://mme.jianghu66.top

Py:   sys.exit(1)
来源：http://qai.hfpthk.cn

PHP:  exit(1);
来源：http://zsn.tanke756.top

JS:   process.exit(1)
来源：http://nxr.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://ewo.nanxinkj.top

Java: System.exit(1)
来源：http://aay.yuanzhike.top

Go:   os.Exit(1)
来源：http://jjl.xziqi.cn

Ruby: exit 1
来源：http://vmk.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zdb.xziqi.cn

[M06] 向标准错误输出
来源：http://hca.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://xyz.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wqg.shzxlz.cn

JS:   console.error("err")
来源：http://hco.dianchejie.cn

TS:   console.error("err")
来源：http://hdy.cashguo.top

Java: System.err.println("err")
来源：http://pmm.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://umf.ivvv.top

Ruby: warn "err"
来源：http://ciy.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://bti.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://qwb.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://blk.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ika.zhixingplan.top

JS:   require.main === module
来源：http://aqt.sjlbkw.cn

TS:   require.main === module
来源：http://hra.yj20258.top

Java: public static void main(String[] args)
来源：http://ruf.epnwcf.com

Go:   func main()
来源：http://dth.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vnh.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://mrt.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://sfe.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://uoc.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://qic.yongpay.top

JS:   process.platform;  process.version
来源：http://jzt.andypj.xyz

TS:   process.platform;  process.version
来源：http://aev.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ozs.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://cml.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xnc.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mgt.zhaomingkeji.xyz

================================================================================
来源：http://sfe.cashguo.top

N. 数据结构与算法
来源：http://bxz.sufxvd.cn

================================================================================
来源：http://jld.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://otz.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://yda.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zef.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://npv.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ecb.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://wzf.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://xfa.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jaz.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://pes.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://glq.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://hrb.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://suf.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yha.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://txp.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kye.meibo888.top

Go:   slices.Sort(arr)
来源：http://nru.sxryk.cn

Ruby: arr.sort
来源：http://wvn.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://opr.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://qvg.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cyt.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://mgv.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://urp.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eoa.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://obf.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://srw.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qkf.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://mta.xziqi.cn

[N04] 斐波那契数列
来源：http://yld.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vcu.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tnb.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gpv.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xhs.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nvb.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wbm.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ugf.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qfg.hywenlv.cn

[N05] 最大公约数
来源：http://nsc.meibo888.top

Py:   math.gcd(a, b)
来源：http://dat.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ldn.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ehd.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eml.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ixh.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sbq.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://pmt.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ldw.nwbrower.top

[N06] 判断回文字符串
来源：http://nte.nanxinkj.top

Py:   s == s[::-1]
来源：http://ftq.xziqi.cn

PHP:  $s === strrev($s);
来源：http://txt.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://wek.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://wxg.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tux.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://ktu.jqgfzy.top

Ruby: s == s.reverse
来源：http://ant.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rlz.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://lxy.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://idz.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ynr.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://fty.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://sie.hesvh.cn

Java: // 手写 HashMap
来源：http://sow.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://vti.zhengqikj.top

Ruby: // 手写 Hash
来源：http://qkw.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ykz.jinqigfzy.top

[N08] 生成全排列
来源：http://wkn.guowangkeji.top


<!-- 参考信息 -->