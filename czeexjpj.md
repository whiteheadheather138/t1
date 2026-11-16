代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://eif.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uax.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fzx.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rwt.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ceq.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gyl.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nxw.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bca.zhiwuduotai.top

================================================================================
来源：http://dde.redwolf501.top

K. JSON 与序列化
来源：http://sjf.sysykeji.top

================================================================================
来源：http://kag.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://nir.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ngp.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vqh.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://eon.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://ixx.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iyn.fehbvm.com

Go:   json.Marshal(obj)
来源：http://bnr.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://omx.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://roq.epnwcf.com

[K02] JSON 字符串转对象
来源：http://nti.cucudq.cn

Py:   json.loads(s)
来源：http://ixu.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vem.haohaochexian.top

JS:   JSON.parse(s)
来源：http://zam.sxryk.cn

TS:   JSON.parse(s)
来源：http://dkm.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jry.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://szx.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://rmu.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lop.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://zez.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sxs.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rig.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://adw.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://uci.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xoy.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zcn.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://faw.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nwl.yuxming.cn

[K04] 读取 JSON 文件
来源：http://qbi.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jjp.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yhq.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aht.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zjd.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mfp.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rsk.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://aor.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oki.smart0.xyz

[K05] 深拷贝对象
来源：http://tld.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://jnl.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://uji.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://jpa.epnwcf.com

TS:   structuredClone(obj)
来源：http://jsj.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://who.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eyf.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zfk.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mjj.gzhubu.top

[K06] 解析 URL 查询串
来源：http://kuw.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://frm.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pds.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jec.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqd.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ggz.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://prh.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fcz.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dzc.gaohongyu789.top

[K07] 进制转换
来源：http://zzg.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nyq.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jmz.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ncg.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lhq.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hvf.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gbb.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yio.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rsx.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://sgm.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://hdw.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://orl.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://axv.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://mde.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pbl.xuanzx.com

Go:   encoding/gob
来源：http://oyt.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://zjy.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qwa.tarul.cn

================================================================================
来源：http://cud.zhixingplan.top

L. 网络请求
来源：http://cye.shanyushiyangkeji.top

================================================================================
来源：http://pxi.havefunace.top

[L01] 发送 GET 请求
来源：http://tgh.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hcv.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nwf.shuidangran.top

JS:   await fetch(url)
来源：http://pqn.9152youxi.cn

TS:   await fetch(url)
来源：http://cdm.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cgt.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://ief.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jva.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ytf.tian-w.cn

[L02] 发送 POST JSON
来源：http://dor.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rxl.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ubi.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://otl.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://apa.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://byb.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qhm.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yny.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vab.sufxvd.cn

[L03] 设置自定义请求头
来源：http://phr.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://obh.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eqc.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jtj.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://joj.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uqb.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kmq.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://umd.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mgc.pengpengdd.cyou

[L04] 设置超时
来源：http://sox.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://kzb.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xux.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxh.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hgm.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vgg.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nkt.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://atq.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://icf.ydzc1.top

[L05] 上传文件（multipart）
来源：http://vjj.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ivx.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mub.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mzp.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xam.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vzs.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://izp.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bme.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ken.xuanzx.com

[L06] 解析响应为 JSON
来源：http://lhd.bbcook.cn

Py:   resp.json()
来源：http://gfq.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://tdv.fanxiaobao.xyz

JS:   await resp.json()
来源：http://nsc.ybcxt.top

TS:   await resp.json()
来源：http://vua.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tel.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wed.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://pzg.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sfk.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://qei.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rfc.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zvd.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://yed.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://xkt.uphjek.com

Java: resp.statusCode()
来源：http://ogu.hfpthk.cn

Go:   resp.StatusCode
来源：http://rwj.shzxlz.cn

Ruby: resp.code.to_i
来源：http://xxx.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://qqd.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://sse.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ewv.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://llm.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fho.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpd.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://abm.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pnt.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tbz.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rrk.hammf.cn

================================================================================
来源：http://sgb.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://dql.wangdashe.top

================================================================================
来源：http://iau.yonumen.top

[M01] 读取命令行参数
来源：http://gca.zdbjq.cn

Py:   sys.argv[1:]
来源：http://ugq.nwbrower.top

PHP:  $argv;  $argc;
来源：http://ulw.gzhubu.top

JS:   process.argv.slice(2)
来源：http://yxj.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://jmm.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://eqi.guannengcc.top

Go:   os.Args[1:]
来源：http://pun.hnqzz.top

Ruby: ARGV
来源：http://moq.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://uwb.jianghu66.top

[M02] 读取环境变量
来源：http://sch.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://bok.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hkd.wangdashe.top

JS:   process.env.HOME
来源：http://abn.yanxiufei.cn

TS:   process.env.HOME
来源：http://poc.tanke756.top

Java: System.getenv("HOME")
来源：http://izx.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jwm.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://eep.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lnv.snrcjt.cn

[M03] 执行外部命令
来源：http://hns.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bwv.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://url.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bqe.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yas.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gcf.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jya.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://xxj.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://uug.ivvv.top

[M04] 获取当前工作目录
来源：http://aba.zhoulong.xyz

Py:   os.getcwd()
来源：http://jvv.bjfxy.top

PHP:  getcwd();
来源：http://aoq.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://qeu.yongpay.top

TS:   process.cwd()
来源：http://oby.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://hil.svipenyu.cn

Go:   os.Getwd()
来源：http://mkm.chenlongwang.top

Ruby: Dir.pwd
来源：http://qow.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://rte.quarkkingdee.top

[M05] 设置退出码
来源：http://jqz.fktsv.cn

Py:   sys.exit(1)
来源：http://zbg.havefunace.top

PHP:  exit(1);
来源：http://ydc.ehwqpu.com

JS:   process.exit(1)
来源：http://vjs.tian-w.cn

TS:   process.exit(1)
来源：http://kvf.yanxiufei.cn

Java: System.exit(1)
来源：http://vec.gzhubu.top

Go:   os.Exit(1)
来源：http://ipj.ctjpmb.com

Ruby: exit 1
来源：http://hdi.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://veg.hnqzz.top

[M06] 向标准错误输出
来源：http://krb.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://fpk.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wpf.zhixingplan.top

JS:   console.error("err")
来源：http://qjn.yuxming.cn

TS:   console.error("err")
来源：http://ccc.9152youxi.cn

Java: System.err.println("err")
来源：http://ttv.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cjm.yonumen.top

Ruby: warn "err"
来源：http://ucz.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://zly.yj20258888.top

[M07] 判断是否为主入口
来源：http://wvj.meibo888.top

Py:   if __name__ == "__main__":
来源：http://odt.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yws.tianlin.xyz

JS:   require.main === module
来源：http://dhb.guannengcc.top

TS:   require.main === module
来源：http://nzb.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://vad.zhiwuduotai.top

Go:   func main()
来源：http://nzf.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tcr.xuanzx.com

C#:   static void Main(string[] args)
来源：http://zpt.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://rhs.andypj.xyz

Py:   platform.system();  platform.python_version()
来源：http://zgx.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://gbo.ivvv.top

JS:   process.platform;  process.version
来源：http://snl.ivvv.top

TS:   process.platform;  process.version
来源：http://rpu.haohaochexian.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dms.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sft.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://was.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://tkp.jinqigfzy.top

================================================================================
来源：http://baq.zhijiandao.cn

N. 数据结构与算法
来源：http://kyo.iojbl.cn

================================================================================
来源：http://wna.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://ktp.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://vnl.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mdm.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ztk.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://drs.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://ctt.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://lgt.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oqv.gogol.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://soj.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://wyc.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://cvs.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ssb.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jpy.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rip.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://geh.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://nio.snrcjt.cn

Ruby: arr.sort
来源：http://pfi.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bqt.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://slv.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xzq.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://nix.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bps.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qyl.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eri.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pyj.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nzd.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zls.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://lzk.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kwp.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://odi.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zxo.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xql.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fph.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kcp.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ups.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ogg.epnwcf.com

[N05] 最大公约数
来源：http://wuf.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://yql.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vyk.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxj.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gov.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://txv.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wgq.gaohongyu789.top

Ruby: a.gcd(b)
来源：http://dtj.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fvz.sxryk.cn

[N06] 判断回文字符串
来源：http://zsm.ydjk.org.cn

Py:   s == s[::-1]
来源：http://tvd.fengsongda.top

PHP:  $s === strrev($s);
来源：http://ptf.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://cej.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://evv.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tln.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://nne.cashguo.top

Ruby: s == s.reverse
来源：http://cfa.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tjs.yj20258.top

[N07] 两数之和（返回下标）
来源：http://qhm.guowangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yfp.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xku.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://yec.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://epj.nanxinkj.top

Java: // 手写 HashMap
来源：http://uuc.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://jgt.yuanzhike.top

Ruby: // 手写 Hash
来源：http://vla.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pyo.shanyushiyangtech.top

[N08] 生成全排列
来源：http://acr.svipenyu.cn


<!-- 参考信息 -->