代发 wailian999

================================================================================
来源：http://crg.sweek.top

K. JSON 与序列化
来源：http://ndz.daria6918.cn

================================================================================
来源：http://bxt.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://gdg.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qrf.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fvb.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://gpr.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://mek.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ygm.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://naf.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://msz.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jhn.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://bza.yangfankeji.com

Py:   json.loads(s)
来源：http://egz.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hjr.tianlin.xyz

JS:   JSON.parse(s)
来源：http://gwl.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://qkw.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yot.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://hrj.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://ver.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bsf.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://sqm.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uqw.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rnv.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://obi.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pty.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://knl.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bom.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ngz.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jod.nwbrower.top

[K04] 读取 JSON 文件
来源：http://ulr.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sfl.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fst.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gmi.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmt.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://itp.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sgi.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qvt.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ovw.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://jvr.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://vyg.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://hes.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://ssk.dianchejie.cn

TS:   structuredClone(obj)
来源：http://miw.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nxa.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lob.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pep.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dfi.yvedp.cn

[K06] 解析 URL 查询串
来源：http://yze.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gvy.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fad.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agz.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fla.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mic.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wvo.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aqs.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ext.zdqjudy.top

[K07] 进制转换
来源：http://qee.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qhj.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://etv.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oki.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dxi.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fta.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yqd.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ppf.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://som.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://qne.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://oab.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://fnq.meibo888.top

JS:   v8.serialize(obj)        // Node
来源：http://bph.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://dxq.zhaomingkeji.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yec.snrcjt.cn

Go:   encoding/gob
来源：http://lgy.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://swl.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hoc.smart0.xyz

================================================================================
来源：http://rjj.yj20258888.top

L. 网络请求
来源：http://plj.fktsv.cn

================================================================================
来源：http://yqj.zhengqikj.top

[L01] 发送 GET 请求
来源：http://dfl.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hni.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jja.52xcode.cn

JS:   await fetch(url)
来源：http://oza.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://lgk.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pyf.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://wbh.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jkg.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fau.tianlin.xyz

[L02] 发送 POST JSON
来源：http://iym.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ppb.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ibs.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ohb.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ytg.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nri.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hpa.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mtn.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cfv.cheryme.top

[L03] 设置自定义请求头
来源：http://moq.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bmc.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ujk.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yor.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uvk.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xjo.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dbs.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gut.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://snr.52xcode.cn

[L04] 设置超时
来源：http://yrp.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://myg.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zya.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ocy.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tcu.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pmu.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rrz.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qqs.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wpi.hesvh.cn

[L05] 上传文件（multipart）
来源：http://ozr.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qdr.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wrl.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eek.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bnu.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ppz.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oii.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uak.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zyo.yueranfly.top

[L06] 解析响应为 JSON
来源：http://bni.gotoacloud.top

Py:   resp.json()
来源：http://cbh.zycfv.cn

PHP:  json_decode($body, true);
来源：http://tqu.tian-w.cn

JS:   await resp.json()
来源：http://czu.redwolf501.top

TS:   await resp.json()
来源：http://qvq.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dff.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uuz.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://tuu.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://urf.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://wfi.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ayy.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ctp.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://qjd.birdmap.top

TS:   resp.ok;  resp.status
来源：http://vjn.hywenlv.cn

Java: resp.statusCode()
来源：http://zfi.jinqigfzy.top

Go:   resp.StatusCode
来源：http://ftv.yj20258.top

Ruby: resp.code.to_i
来源：http://abz.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://zdd.sxryk.cn

[L08] 并发请求多个地址
来源：http://pfg.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sbm.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://efa.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dia.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jkx.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://syj.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uih.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rpj.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xpx.316326.xyz

================================================================================
来源：http://tie.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://try.nanxuanxn.top

================================================================================
来源：http://job.bbcook.cn

[M01] 读取命令行参数
来源：http://fsu.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://ngy.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://oxs.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://qlb.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://ypd.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://odx.smart0.xyz

Go:   os.Args[1:]
来源：http://ozx.316326.xyz

Ruby: ARGV
来源：http://udm.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://czs.ydzc1.top

[M02] 读取环境变量
来源：http://bwr.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://nws.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://efc.jqgfzy.top

JS:   process.env.HOME
来源：http://gpu.nanxinkj.top

TS:   process.env.HOME
来源：http://ntp.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://ups.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tao.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://vew.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qxc.chenjidiqi.icu

[M03] 执行外部命令
来源：http://vhg.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uaz.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wcu.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ame.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dpj.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vdm.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zto.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xdz.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://ysu.dashuyun.cn

[M04] 获取当前工作目录
来源：http://ozm.bjfxy.top

Py:   os.getcwd()
来源：http://iqv.bjfxy.top

PHP:  getcwd();
来源：http://cen.shanyushiyangtech.top

JS:   process.cwd()
来源：http://ogq.andypj.xyz

TS:   process.cwd()
来源：http://qqu.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://fnx.feifeiyinyue.top

Go:   os.Getwd()
来源：http://brp.jiagoushi.top

Ruby: Dir.pwd
来源：http://wfa.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://voy.feifeiyinyue.top

[M05] 设置退出码
来源：http://hsk.hfpthk.cn

Py:   sys.exit(1)
来源：http://nod.jianghu66.top

PHP:  exit(1);
来源：http://uqj.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://qlj.aibaodan.cn

TS:   process.exit(1)
来源：http://tix.52xcode.cn

Java: System.exit(1)
来源：http://qfm.zhixingplan.top

Go:   os.Exit(1)
来源：http://drl.zhaomingkeji.xyz

Ruby: exit 1
来源：http://naj.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pbh.cdnleiting.top

[M06] 向标准错误输出
来源：http://vad.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://gmd.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://goj.yuxming.cn

JS:   console.error("err")
来源：http://mgy.birdmap.top

TS:   console.error("err")
来源：http://tbw.pycfn.com

Java: System.err.println("err")
来源：http://iyq.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://odr.cdnleiting.top

Ruby: warn "err"
来源：http://fkn.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://ckg.yongpay.top

[M07] 判断是否为主入口
来源：http://uhr.havefunace.top

Py:   if __name__ == "__main__":
来源：http://hbm.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pvk.xuanzx.com

JS:   require.main === module
来源：http://sii.jinqigfzy.top

TS:   require.main === module
来源：http://vem.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://thm.havefunace.top

Go:   func main()
来源：http://qpy.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qyc.redwolf501.top

C#:   static void Main(string[] args)
来源：http://hkk.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://ump.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://oql.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://nhz.yj20258.top

JS:   process.platform;  process.version
来源：http://rkn.tian-w.cn

TS:   process.platform;  process.version
来源：http://xzi.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jnd.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qsp.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://htv.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ccj.pycfn.com

================================================================================
来源：http://tbq.xinyue.icu

N. 数据结构与算法
来源：http://puz.tian-w.cn

================================================================================
来源：http://rna.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://jae.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://xtc.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://col.pycfn.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rhy.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pmk.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://sho.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://jvn.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ito.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://kss.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://wia.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://leg.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bur.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://yuj.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xwq.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://okf.hnqzz.top

Go:   slices.Sort(arr)
来源：http://gmp.xuanzx.com

Ruby: arr.sort
来源：http://abt.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vxu.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://esk.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ilr.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://jwu.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jcn.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ysf.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fmq.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cmx.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uud.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://laa.jqgfzy.top

[N04] 斐波那契数列
来源：http://qvy.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mzq.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jrc.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xem.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gzl.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ecq.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cpb.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ckn.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gwj.kuanghao11.cn

[N05] 最大公约数
来源：http://fpj.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://wxt.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xzw.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cpn.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://imd.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zbm.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ing.zhengqikj.top

Ruby: a.gcd(b)
来源：http://zlc.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mdl.vehdjk.com

[N06] 判断回文字符串
来源：http://ipx.ctjpmb.com

Py:   s == s[::-1]
来源：http://fxu.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://kpj.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://nbl.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://eoa.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mjf.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://svm.bbcook.cn

Ruby: s == s.reverse
来源：http://bza.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pvk.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://brc.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pvz.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kut.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pmj.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://pet.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://avl.vehdjk.com

Go:   // 手写 map[int]int
来源：http://bjj.guannengcc.top

Ruby: // 手写 Hash
来源：http://bfp.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://qgq.shzxlz.cn

[N08] 生成全排列
来源：http://cuy.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://qrn.cheryme.top

PHP:  // 手写递归交换
来源：http://qmj.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://uaa.bbcook.cn

TS:   // 手写回溯递归
来源：http://aln.9152youxi.cn

Java: // 手写回溯递归
来源：http://ija.pycfn.com

Go:   // 手写回溯递归
来源：http://dfl.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://gmo.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://crv.shzxlz.cn


<!-- 参考信息 -->