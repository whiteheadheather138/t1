代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://phd.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ukk.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qxf.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://apo.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ovz.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bnt.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uwc.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ylw.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gqx.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pat.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kyh.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aze.hammf.cn

================================================================================
来源：http://ksf.aizwys.cn

K. JSON 与序列化
来源：http://xdt.vehdjk.com

================================================================================
来源：http://hhd.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://xmn.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ple.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ubt.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://znq.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://mak.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jcq.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://mrl.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://xqr.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vja.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://ioy.ybcxt.top

Py:   json.loads(s)
来源：http://xrr.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gkx.ivvv.top

JS:   JSON.parse(s)
来源：http://psk.dianchejie.cn

TS:   JSON.parse(s)
来源：http://tye.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tqt.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://khh.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://ypq.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ypl.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://fqn.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gcb.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yad.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bip.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ppt.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wtk.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nzh.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kyt.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uhm.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://umj.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tas.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xug.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eks.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://juf.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sxn.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ude.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pxf.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ire.zdbjq.cn

[K05] 深拷贝对象
来源：http://feu.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://aig.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://mbk.dashuyun.cn

JS:   structuredClone(obj)
来源：http://vve.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://zyb.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://piv.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dlb.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ath.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mov.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://qjr.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qfe.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yme.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hgv.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xeh.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://evx.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://odp.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wxr.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cvk.kuanghao11.cn

[K07] 进制转换
来源：http://bnc.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yuf.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nnq.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://une.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ukp.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://egw.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qys.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xnj.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rtf.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://dji.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://zfd.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iup.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://oid.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://eav.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dsa.vehdjk.com

Go:   encoding/gob
来源：http://zgm.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://enq.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kur.tarul.cn

================================================================================
来源：http://ofy.fanxiaobao.xyz

L. 网络请求
来源：http://pch.fehbvm.com

================================================================================
来源：http://yor.nanxinkj.top

[L01] 发送 GET 请求
来源：http://bsm.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yrv.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wuo.pycfn.com

JS:   await fetch(url)
来源：http://ngy.gzhubu.top

TS:   await fetch(url)
来源：http://hix.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://olv.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://ncf.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vgb.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hwg.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://qdi.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://klx.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://soh.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gmh.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://icm.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sik.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ndo.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yyr.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xlg.xziqi.cn

[L03] 设置自定义请求头
来源：http://mpn.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vxh.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bor.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewk.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yto.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wvm.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fnl.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zpv.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hgc.jinghuilouyu.cn

[L04] 设置超时
来源：http://nfd.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://fyn.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qvg.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xen.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zzu.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wax.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://alx.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kjl.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ype.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://bcn.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://srs.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mmw.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eal.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://phb.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jlx.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uio.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ydm.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wvx.yongpay.top

[L06] 解析响应为 JSON
来源：http://qip.xinyue.icu

Py:   resp.json()
来源：http://krp.gzhubu.top

PHP:  json_decode($body, true);
来源：http://hql.tianlin.xyz

JS:   await resp.json()
来源：http://rei.316326.xyz

TS:   await resp.json()
来源：http://kfd.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zyu.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cjn.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://swb.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hwm.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://xqt.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zjo.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nva.meibo888.top

JS:   resp.ok;  resp.status
来源：http://lyp.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://kls.52xcode.cn

Java: resp.statusCode()
来源：http://miv.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://jiu.tianlin.xyz

Ruby: resp.code.to_i
来源：http://rwt.havefunace.top

C#:   (int)resp.StatusCode
来源：http://pdn.wangdashe.top

[L08] 并发请求多个地址
来源：http://dah.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kfc.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://smy.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sss.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsa.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gso.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mzg.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kyr.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://luq.ydjk.org.cn

================================================================================
来源：http://mww.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://ulc.vqdsnc.cn

================================================================================
来源：http://kvf.ybcxt.top

[M01] 读取命令行参数
来源：http://mul.chenlongwang.top

Py:   sys.argv[1:]
来源：http://jco.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://vjf.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://nms.pycfn.com

TS:   process.argv.slice(2)
来源：http://hap.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://znl.vqdsnc.cn

Go:   os.Args[1:]
来源：http://ram.bjfxy.top

Ruby: ARGV
来源：http://uwa.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://ard.zdqjudy.top

[M02] 读取环境变量
来源：http://bwp.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://uuj.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yeb.fzhhl.top

JS:   process.env.HOME
来源：http://ozy.snrcjt.cn

TS:   process.env.HOME
来源：http://cat.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://ejs.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ojj.gzhubu.top

Ruby: ENV["HOME"]
来源：http://pwj.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cmx.xylfe.cn

[M03] 执行外部命令
来源：http://kbe.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hzv.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ysh.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rvd.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yav.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wko.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://swj.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://xps.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://xin.dashuyun.cn

[M04] 获取当前工作目录
来源：http://yot.cucudq.cn

Py:   os.getcwd()
来源：http://dox.xinyue.icu

PHP:  getcwd();
来源：http://nso.cqqwz.cn

JS:   process.cwd()
来源：http://jto.guannengcc.top

TS:   process.cwd()
来源：http://tso.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://tpj.daria6918.cn

Go:   os.Getwd()
来源：http://rcy.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://uwb.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://prn.quarkkingdee.top

[M05] 设置退出码
来源：http://nhw.vehdjk.com

Py:   sys.exit(1)
来源：http://sjj.9152youxi.cn

PHP:  exit(1);
来源：http://lzj.epnwcf.com

JS:   process.exit(1)
来源：http://dfx.sxryk.cn

TS:   process.exit(1)
来源：http://izf.daria6918.cn

Java: System.exit(1)
来源：http://wdl.ivvv.top

Go:   os.Exit(1)
来源：http://hxp.xziqi.cn

Ruby: exit 1
来源：http://own.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://flx.kuanghao11.cn

[M06] 向标准错误输出
来源：http://bqx.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://gpy.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zom.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://wqd.yonumen.top

TS:   console.error("err")
来源：http://uao.wangdashe.top

Java: System.err.println("err")
来源：http://qae.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zvr.daxiang520.top

Ruby: warn "err"
来源：http://alt.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://cfw.cheryme.top

[M07] 判断是否为主入口
来源：http://cde.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://bev.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kzc.yj202588.top

JS:   require.main === module
来源：http://ylx.mhx1999.top

TS:   require.main === module
来源：http://pwm.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://fkz.yfazqb.com

Go:   func main()
来源：http://twz.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kxy.redwolf501.top

C#:   static void Main(string[] args)
来源：http://taj.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://jdg.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://aot.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://pwj.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://apa.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://ril.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qzn.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yju.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rft.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vqk.chenlongwang.top

================================================================================
来源：http://ejx.bbcook.cn

N. 数据结构与算法
来源：http://tqb.zhongyouzk.top

================================================================================
来源：http://yrm.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://jkw.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://ayl.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zqy.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ubj.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urq.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pal.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://pmh.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gey.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://ayv.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://sck.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://wiv.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lbo.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ydm.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vqm.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pwu.gzhubu.top

Go:   slices.Sort(arr)
来源：http://pur.c1oappe.top

Ruby: arr.sort
来源：http://auy.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cvf.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://hwq.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sko.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://cbu.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dwd.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://meb.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://srl.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://umm.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ayc.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zwe.jinqigfzy.top

[N04] 斐波那契数列
来源：http://hyo.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://two.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kig.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lok.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lcw.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xrq.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jii.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://csi.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yed.ivvv.top

[N05] 最大公约数
来源：http://ysn.yuxming.cn

Py:   math.gcd(a, b)
来源：http://hhq.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ijl.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://utr.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvt.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ehw.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zxf.yvedp.cn

Ruby: a.gcd(b)
来源：http://uwc.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bel.hnxiangtu.top

[N06] 判断回文字符串
来源：http://bcu.kuanghao11.cn

Py:   s == s[::-1]
来源：http://jwr.yfazqb.com

PHP:  $s === strrev($s);
来源：http://izx.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://jae.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://euw.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rdl.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://ikm.fengsongda.top

Ruby: s == s.reverse
来源：http://cpz.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wlr.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://keg.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ify.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rcn.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fuo.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://gvr.shuidangran.top

Java: // 手写 HashMap
来源：http://who.ppjwa.cn


<!-- 参考信息 -->