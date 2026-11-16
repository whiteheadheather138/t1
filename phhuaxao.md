代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wsx.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://wxg.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gyi.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://dhq.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bvc.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eln.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lzh.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://amp.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xbe.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rnb.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://glj.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ujl.xuanzx.com

================================================================================
来源：http://qon.xylfe.cn

K. JSON 与序列化
来源：http://hhy.yj20258888.top

================================================================================
来源：http://pwp.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://ldi.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://buq.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zzb.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://mhf.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://oyu.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lks.yj20258.top

Go:   json.Marshal(obj)
来源：http://qwu.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://ive.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cnx.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://lsb.yfazqb.com

Py:   json.loads(s)
来源：http://phm.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://arf.dashuyun.cn

JS:   JSON.parse(s)
来源：http://mmi.xylfe.cn

TS:   JSON.parse(s)
来源：http://dsj.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://auw.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://sbr.yuxming.cn

Ruby: JSON.parse(s)
来源：http://llq.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ghs.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://eta.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zye.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bhu.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zzn.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nga.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qoq.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jbh.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://jyt.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://whr.316326.xyz

[K04] 读取 JSON 文件
来源：http://pit.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aff.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rbn.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hnc.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgn.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://emv.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cvk.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yxy.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oqu.wangdashe.top

[K05] 深拷贝对象
来源：http://ynw.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://rst.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://qzr.fktsv.cn

JS:   structuredClone(obj)
来源：http://omp.haohaochexian.top

TS:   structuredClone(obj)
来源：http://wbp.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ndw.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wsc.jiagoushi.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qme.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ndg.cheryme.top

[K06] 解析 URL 查询串
来源：http://qwt.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yir.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vxh.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bky.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzw.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iou.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mmk.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bpo.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dnm.zhengqikj.top

[K07] 进制转换
来源：http://pad.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tnu.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uum.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ufu.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kki.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cws.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ukt.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eek.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xaw.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://xis.havefunace.top

Py:   pickle.dumps(obj)
来源：http://pwp.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nwr.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://npu.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://olt.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vof.aizwys.cn

Go:   encoding/gob
来源：http://xwb.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://uvq.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://azo.yvedp.cn

================================================================================
来源：http://yca.zdbjq.cn

L. 网络请求
来源：http://fun.epnwcf.com

================================================================================
来源：http://rrz.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://hnk.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wdv.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fdf.zhengqikj.top

JS:   await fetch(url)
来源：http://siw.nanxinkj.top

TS:   await fetch(url)
来源：http://zqz.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eoe.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://ffo.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pgd.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://css.ivvv.top

[L02] 发送 POST JSON
来源：http://zms.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dsy.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sdi.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lyc.cdnleiting.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yzz.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://suv.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bhd.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ucp.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://asw.tian-w.cn

[L03] 设置自定义请求头
来源：http://cgc.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jlc.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fvk.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xiz.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkn.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fxf.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uue.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://got.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lpr.yueranfly.top

[L04] 设置超时
来源：http://azm.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://ulp.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ysp.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ugh.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rwx.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ikx.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oqd.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fmx.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ams.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://goq.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ujy.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kub.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gjd.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lvl.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xua.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xfm.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qos.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://txi.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://dqj.daria6918.cn

Py:   resp.json()
来源：http://mqz.316326.xyz

PHP:  json_decode($body, true);
来源：http://ztd.chenjidiqi.icu

JS:   await resp.json()
来源：http://kwy.ybcxt.top

TS:   await resp.json()
来源：http://lcf.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sig.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://swr.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://jyx.jinyuanbaomall.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xjj.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://six.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://skt.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bag.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://gki.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://epj.zhijiandao.cn

Java: resp.statusCode()
来源：http://uyw.zhoulong.xyz

Go:   resp.StatusCode
来源：http://mut.wangdashe.top

Ruby: resp.code.to_i
来源：http://pnf.hfpthk.cn

C#:   (int)resp.StatusCode
来源：http://bdg.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://sfy.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jtc.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://qqj.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xqf.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nkh.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hag.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ktd.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ojo.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pfw.sweek.top

================================================================================
来源：http://zoo.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://yuq.dashuyun.cn

================================================================================
来源：http://faz.daria6918.cn

[M01] 读取命令行参数
来源：http://doz.hysaishi.cn

Py:   sys.argv[1:]
来源：http://scj.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://kre.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://yzy.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://hka.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://wks.ivvv.top

Go:   os.Args[1:]
来源：http://ytq.yanxiufei.cn

Ruby: ARGV
来源：http://jtm.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://bqk.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://dqt.uphjek.com

Py:   os.environ.get("HOME")
来源：http://nnx.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://krl.ydjk.org.cn

JS:   process.env.HOME
来源：http://xke.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://mvg.jianghu66.top

Java: System.getenv("HOME")
来源：http://ukm.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qoz.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://pgi.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ndx.yongpay.top

[M03] 执行外部命令
来源：http://jyt.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkb.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://abn.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dpv.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pnu.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gjx.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://blb.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jbb.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://vnp.haohaochexian.top

[M04] 获取当前工作目录
来源：http://aad.hysaishi.cn

Py:   os.getcwd()
来源：http://nih.sweek.top

PHP:  getcwd();
来源：http://xgv.ydjk.org.cn

JS:   process.cwd()
来源：http://uua.jianghu66.top

TS:   process.cwd()
来源：http://ryv.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://wwh.wangshuangyany.cn

Go:   os.Getwd()
来源：http://yzl.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://bfr.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://gav.bjfxy.top

[M05] 设置退出码
来源：http://qde.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://bvo.nwbrower.top

PHP:  exit(1);
来源：http://ccz.shuidangran.top

JS:   process.exit(1)
来源：http://vdg.bbcook.cn

TS:   process.exit(1)
来源：http://wwj.cheryme.top

Java: System.exit(1)
来源：http://wgg.svipenyu.cn

Go:   os.Exit(1)
来源：http://zlz.zhoulong.xyz

Ruby: exit 1
来源：http://fdg.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oci.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://icm.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://vhw.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mlz.hysaishi.cn

JS:   console.error("err")
来源：http://zpc.bjfxy.top

TS:   console.error("err")
来源：http://qfj.ehwqpu.com

Java: System.err.println("err")
来源：http://uyo.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jxt.fanxiaobao.xyz

Ruby: warn "err"
来源：http://bmh.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://mnf.zhengqikj.top

[M07] 判断是否为主入口
来源：http://mfy.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://cwy.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xwg.52xcode.cn

JS:   require.main === module
来源：http://cws.yongpay.top

TS:   require.main === module
来源：http://iqn.epnwcf.com

Java: public static void main(String[] args)
来源：http://mqv.zhixingplan.top

Go:   func main()
来源：http://iqj.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mzp.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://mfe.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://lth.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://syj.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://hrq.yuxming.cn

JS:   process.platform;  process.version
来源：http://oxq.zdqjudy.top

TS:   process.platform;  process.version
来源：http://mjm.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ihj.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rhf.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xha.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dyc.ywan-chungtsiang.top

================================================================================
来源：http://bde.jinghuilouyu.cn

N. 数据结构与算法
来源：http://wce.jinqigfzy.top

================================================================================
来源：http://raa.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://fag.yangfankeji.com

Py:   bisect.bisect_left(arr, x)
来源：http://twz.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rbe.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://djd.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://suq.yueranfly.top

Java: Arrays.binarySearch(arr, x)
来源：http://ctu.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://nmb.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://brv.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uey.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://kqg.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://kja.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sab.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jww.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lfb.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bkg.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://qyu.gaohongyu789.top

Ruby: arr.sort
来源：http://oyz.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wta.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://xfk.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gaz.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://fuw.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lwe.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hid.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kyn.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://prj.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hsd.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://dgg.yueranfly.top

[N04] 斐波那契数列
来源：http://acs.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qhs.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gfw.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mih.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pug.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hqo.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ctt.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bsn.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zsz.cheryme.top

[N05] 最大公约数
来源：http://gse.fzhhl.top

Py:   math.gcd(a, b)
来源：http://bja.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hts.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oxk.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gqm.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qpy.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hgd.hysaishi.cn

Ruby: a.gcd(b)
来源：http://lnn.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fxh.svipenyu.cn

[N06] 判断回文字符串
来源：http://jag.snrcjt.cn

Py:   s == s[::-1]
来源：http://xcb.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://fzf.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://xbd.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://czk.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rmy.tian-w.cn

Go:   // 双指针从两端比较
来源：http://kcr.fktsv.cn

Ruby: s == s.reverse
来源：http://wxx.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qyd.ivvv.top

[N07] 两数之和（返回下标）
来源：http://qjv.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zok.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://onu.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vyu.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://xpr.yangfankeji.com

Java: // 手写 HashMap
来源：http://xcq.zdqjudy.top


<!-- 参考信息 -->