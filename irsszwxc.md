代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mmb.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lsf.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hhe.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://pbi.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cyg.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ezb.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jnw.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lfx.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yuc.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hfh.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ixo.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xoq.sxryk.cn

================================================================================
来源：http://tqo.hesvh.cn

K. JSON 与序列化
来源：http://meh.tanke756.top

================================================================================
来源：http://qkx.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://kqm.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uvo.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://phg.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://vzi.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://syn.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zzb.fengsongda.top

Go:   json.Marshal(obj)
来源：http://dln.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://znh.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://jya.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://ldg.vqdsnc.cn

Py:   json.loads(s)
来源：http://xuk.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sao.jqgfzy.top

JS:   JSON.parse(s)
来源：http://gmq.aizwys.cn

TS:   JSON.parse(s)
来源：http://eib.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ero.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://ezw.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://wbt.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uak.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://krq.shuidangran.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vsa.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qao.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hpb.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://hrt.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vay.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iny.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://dgj.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bgk.xuanzx.com

[K04] 读取 JSON 文件
来源：http://fmt.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pur.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uqj.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://swa.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lxi.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dyn.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pio.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xlo.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yuq.ybcxt.top

[K05] 深拷贝对象
来源：http://ieg.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://yzk.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://lct.ivvv.top

JS:   structuredClone(obj)
来源：http://edq.hammf.cn

TS:   structuredClone(obj)
来源：http://qdr.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dyb.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qcu.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cyz.cheryme.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hnh.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://psv.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yeh.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lgr.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qlr.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxp.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hbz.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eqn.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eoa.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xje.vehdjk.com

[K07] 进制转换
来源：http://vcn.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mlk.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rak.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://est.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://efm.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ksw.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://poa.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://feu.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://whr.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://dfg.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://ksx.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vjc.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://qfu.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://ort.jinqigfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wrn.hnqzz.top

Go:   encoding/gob
来源：http://xbz.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://acm.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tbe.tianlin.xyz

================================================================================
来源：http://okj.0kj1m.cn

L. 网络请求
来源：http://hbx.cdnleiting.top

================================================================================
来源：http://sqz.chenzaomai.com

[L01] 发送 GET 请求
来源：http://ovv.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rcw.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uqc.chenlongwang.top

JS:   await fetch(url)
来源：http://uxk.cheryme.top

TS:   await fetch(url)
来源：http://orl.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://god.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://qqb.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dra.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pvu.yueranfly.top

[L02] 发送 POST JSON
来源：http://vvy.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://smt.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kyg.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jde.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgg.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://prj.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://msl.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bqt.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://azj.cdnleiting.top

[L03] 设置自定义请求头
来源：http://dck.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dru.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rhm.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cbo.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tvm.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://otb.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sgg.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bwv.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qkk.cucudq.cn

[L04] 设置超时
来源：http://npz.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://lwc.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gwo.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oef.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zqi.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pvd.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ola.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bwc.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ysk.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://mpn.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iuv.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://atm.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://akm.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://goo.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pye.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bzj.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pjf.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eka.zhoulong.xyz

[L06] 解析响应为 JSON
来源：http://jpo.bjfxy.top

Py:   resp.json()
来源：http://alz.zycfv.cn

PHP:  json_decode($body, true);
来源：http://eyo.tianlin.xyz

JS:   await resp.json()
来源：http://dgm.tianlin.xyz

TS:   await resp.json()
来源：http://zol.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://orx.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://owx.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://qwu.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qgq.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://ntd.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fzz.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fyj.meibo888.top

JS:   resp.ok;  resp.status
来源：http://gcw.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://igs.9152youxi.cn

Java: resp.statusCode()
来源：http://fnf.xinyue.icu

Go:   resp.StatusCode
来源：http://kdj.yangfankeji.com

Ruby: resp.code.to_i
来源：http://hmr.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://ppi.c1oappe.top

[L08] 并发请求多个地址
来源：http://kij.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cmi.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://jjr.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zuc.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fmo.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dhm.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fvn.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rsb.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vyz.ppjwa.cn

================================================================================
来源：http://orf.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://nct.tian-w.cn

================================================================================
来源：http://bqb.zycfv.cn

[M01] 读取命令行参数
来源：http://fwz.bjfxy.top

Py:   sys.argv[1:]
来源：http://ltp.shuidangran.top

PHP:  $argv;  $argc;
来源：http://brr.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://tqe.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://day.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://msl.ctjpmb.com

Go:   os.Args[1:]
来源：http://jgg.hcnkem.com

Ruby: ARGV
来源：http://ian.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://twv.pengpengdd.cyou

[M02] 读取环境变量
来源：http://jwu.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://lsj.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bhd.aizwys.cn

JS:   process.env.HOME
来源：http://bos.0kj1m.cn

TS:   process.env.HOME
来源：http://nax.ybcxt.top

Java: System.getenv("HOME")
来源：http://vek.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bpn.mhx1999.top

Ruby: ENV["HOME"]
来源：http://cyf.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sva.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://oav.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kuc.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mrc.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://szl.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://syn.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://juj.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rbh.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://rpp.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://lvb.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://tcw.hcnkem.com

Py:   os.getcwd()
来源：http://ajh.sjlbkw.cn

PHP:  getcwd();
来源：http://rhd.jiagoushi.top

JS:   process.cwd()
来源：http://cmd.jqgufenzy.top

TS:   process.cwd()
来源：http://cxi.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://ejm.ehwqpu.com

Go:   os.Getwd()
来源：http://mte.uphjek.com

Ruby: Dir.pwd
来源：http://dyg.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://xsd.yj20258888.top

[M05] 设置退出码
来源：http://cui.xuanzx.com

Py:   sys.exit(1)
来源：http://dpn.ydzc1.top

PHP:  exit(1);
来源：http://uhd.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://vhk.meibo888.top

TS:   process.exit(1)
来源：http://ecy.sufxvd.cn

Java: System.exit(1)
来源：http://zki.redwolf501.top

Go:   os.Exit(1)
来源：http://uio.316326.xyz

Ruby: exit 1
来源：http://uyf.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zfm.tarul.cn

[M06] 向标准错误输出
来源：http://dei.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://zlj.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sej.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://chh.hnqzz.top

TS:   console.error("err")
来源：http://gbc.cucudq.cn

Java: System.err.println("err")
来源：http://pqf.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://byt.cheryme.top

Ruby: warn "err"
来源：http://zli.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://ysd.xziqi.cn

[M07] 判断是否为主入口
来源：http://old.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://ihe.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://txv.wangdashe.top

JS:   require.main === module
来源：http://bly.c1oappe.top

TS:   require.main === module
来源：http://udg.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://cgl.hnxiangtu.top

Go:   func main()
来源：http://req.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zfj.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://ltm.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://wde.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://zyr.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://ucr.smart0.xyz

JS:   process.platform;  process.version
来源：http://fvf.gotoacloud.top

TS:   process.platform;  process.version
来源：http://sxb.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qsu.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vwa.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ebq.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zwe.zhongyouzk.top

================================================================================
来源：http://dxq.cqqwz.cn

N. 数据结构与算法
来源：http://qme.jiagoushi.top

================================================================================
来源：http://vtr.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://blw.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://cfi.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dcj.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://byt.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://opx.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://bac.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://hlb.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qna.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jzc.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://yom.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://jfn.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wow.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qqz.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ngw.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wjw.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://ikk.sjlbkw.cn

Ruby: arr.sort
来源：http://gol.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nqb.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://iif.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://umq.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://ghk.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nld.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ztl.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xhw.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://voe.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://swt.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nsj.sxryk.cn

[N04] 斐波那契数列
来源：http://djl.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hjy.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bxz.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hfc.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mry.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqf.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jbd.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fqn.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hyc.aibaodan.cn

[N05] 最大公约数
来源：http://bhj.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://gol.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vod.fanxiaobao.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vln.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wpn.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ndr.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://crw.ydzc1.top

Ruby: a.gcd(b)
来源：http://bub.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hsz.9152youxi.cn

[N06] 判断回文字符串
来源：http://egd.fktsv.cn

Py:   s == s[::-1]
来源：http://cdt.bjfxy.top

PHP:  $s === strrev($s);
来源：http://bxm.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://vbb.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://qwj.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vrp.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://rly.aizwys.cn

Ruby: s == s.reverse
来源：http://wdx.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fza.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://rgx.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fvs.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rdj.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tjz.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://iuf.iojbl.cn

Java: // 手写 HashMap
来源：http://psy.guannengcc.top


<!-- 参考信息 -->