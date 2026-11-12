代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fft.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://bgf.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dvm.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fqz.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://auf.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://uqe.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kzl.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wut.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://ahf.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ake.yvedp.cn

[K04] 读取 JSON 文件
来源：http://jjr.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ayj.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mwf.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ugd.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qrw.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://egs.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://smx.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fwq.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eiv.gogol.net.cn

[K05] 深拷贝对象
来源：http://oaq.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://dhm.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://mmh.daria6918.cn

JS:   structuredClone(obj)
来源：http://czm.birdmap.top

TS:   structuredClone(obj)
来源：http://yfm.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mek.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cpt.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xbm.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xzn.zhiwuduotai.top

[K06] 解析 URL 查询串
来源：http://gua.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://swo.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hgh.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lvg.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://com.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ntv.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qyt.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zlz.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://api.jinyuanbaomall.cn

[K07] 进制转换
来源：http://byy.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mws.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rgy.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xhj.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gio.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pps.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hoz.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eox.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://azi.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://bvb.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://dif.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://cvy.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://qhs.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://icx.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yhw.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://klf.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://iod.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sai.gaohongyu789.top

================================================================================
来源：http://kog.yangfankeji.com

L. 网络请求
来源：http://dcn.jianghu66.top

================================================================================
来源：http://wsj.iojbl.cn

[L01] 发送 GET 请求
来源：http://sgx.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://snn.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zsn.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://tgl.gotoacloud.top

TS:   await fetch(url)
来源：http://ocy.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fbt.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://erg.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zbs.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zah.pycfn.com

[L02] 发送 POST JSON
来源：http://fzp.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ict.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kkq.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://laz.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hlz.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dbv.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cnc.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pyp.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fon.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://mzr.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kkj.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wwc.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylt.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dcs.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oru.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://saq.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uzr.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wua.fktsv.cn

[L04] 设置超时
来源：http://fhn.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://rjs.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://skf.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://edy.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zlr.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://age.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lfb.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vdy.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://seh.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://ftt.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qus.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://spr.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xvp.jlsjyb.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eyd.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aao.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sun.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://euq.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cqs.fehbvm.com

[L06] 解析响应为 JSON
来源：http://ghc.yuanzhike.top

Py:   resp.json()
来源：http://xqx.pycfn.com

PHP:  json_decode($body, true);
来源：http://njl.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://ycc.jinghuilouyu.cn

TS:   await resp.json()
来源：http://iio.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ckc.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vza.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://mnk.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gvo.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://nya.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sep.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ccp.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://nwy.meibo888.top

TS:   resp.ok;  resp.status
来源：http://zgu.gaohongyu789.top

Java: resp.statusCode()
来源：http://oxm.bjfxy.top

Go:   resp.StatusCode
来源：http://ltm.52xcode.cn

Ruby: resp.code.to_i
来源：http://sqz.pycfn.com

C#:   (int)resp.StatusCode
来源：http://who.yfazqb.com

[L08] 并发请求多个地址
来源：http://lyq.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wzg.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://fpb.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fgc.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rof.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hax.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rhs.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yie.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ecl.dashuyun.cn

================================================================================
来源：http://qnf.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://tqu.svipenyu.cn

================================================================================
来源：http://ycc.0kj1m.cn

[M01] 读取命令行参数
来源：http://tku.zdqjudy.top

Py:   sys.argv[1:]
来源：http://arp.fehbvm.com

PHP:  $argv;  $argc;
来源：http://vqw.daria6918.cn

JS:   process.argv.slice(2)
来源：http://gqy.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://iyo.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://awg.yangfankeji.com

Go:   os.Args[1:]
来源：http://eoo.gzhubu.top

Ruby: ARGV
来源：http://aof.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://fkk.yueranfly.top

[M02] 读取环境变量
来源：http://nya.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://zdw.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zjo.wangdashe.top

JS:   process.env.HOME
来源：http://akr.ctjpmb.com

TS:   process.env.HOME
来源：http://ken.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://eax.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pen.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://uts.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://noh.smart0.xyz

[M03] 执行外部命令
来源：http://dbz.gotoacloud.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ylc.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mvw.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://akh.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nto.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dvt.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kac.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://ppj.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://ktl.jianghu66.top

[M04] 获取当前工作目录
来源：http://gzt.hongshengwenyu.top

Py:   os.getcwd()
来源：http://sbx.ppjwa.cn

PHP:  getcwd();
来源：http://xpa.jqgufenzy.top

JS:   process.cwd()
来源：http://xom.shuidangran.top

TS:   process.cwd()
来源：http://slk.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://kxd.ybcxt.top

Go:   os.Getwd()
来源：http://oxg.gzhubu.top

Ruby: Dir.pwd
来源：http://auh.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://nsj.mhx1999.top

[M05] 设置退出码
来源：http://hsz.uphjek.com

Py:   sys.exit(1)
来源：http://izi.chenjidiqi.icu

PHP:  exit(1);
来源：http://jni.jqgufenzy.top

JS:   process.exit(1)
来源：http://eon.316326.xyz

TS:   process.exit(1)
来源：http://kqx.sufxvd.cn

Java: System.exit(1)
来源：http://gwz.cqqwz.cn

Go:   os.Exit(1)
来源：http://pbw.nanxinkj.top

Ruby: exit 1
来源：http://eob.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nyy.vehdjk.com

[M06] 向标准错误输出
来源：http://ttw.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://kgr.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nyp.bbcook.cn

JS:   console.error("err")
来源：http://ajn.cashguo.top

TS:   console.error("err")
来源：http://kvi.pycfn.com

Java: System.err.println("err")
来源：http://vlr.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sik.9152youxi.cn

Ruby: warn "err"
来源：http://kqc.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://kyv.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://nio.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://wdr.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://erx.fehbvm.com

JS:   require.main === module
来源：http://abl.bjfxy.top

TS:   require.main === module
来源：http://rrv.mhx1999.top

Java: public static void main(String[] args)
来源：http://ylf.cashguo.top

Go:   func main()
来源：http://chg.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vab.sysykeji.top

C#:   static void Main(string[] args)
来源：http://mjz.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://qwf.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://gmu.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://iam.hysaishi.cn

JS:   process.platform;  process.version
来源：http://ybd.shzxlz.cn

TS:   process.platform;  process.version
来源：http://qib.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nfd.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zgs.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://byb.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iwt.nanxuanxn.top

================================================================================
来源：http://phh.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://vqs.yonumen.top

================================================================================
来源：http://lun.yj202588.top

[N01] 二分查找（有序数组）
来源：http://lbf.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xzz.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nix.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lks.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bhj.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://wke.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://gmb.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://azq.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://dun.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://oag.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://fkp.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qjt.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sih.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fml.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zpi.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://xid.sxryk.cn

Ruby: arr.sort
来源：http://boy.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://ksc.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://gid.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ojb.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://zmf.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://air.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qjh.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zqi.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gca.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sig.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dbn.shzxlz.cn

[N04] 斐波那契数列
来源：http://ubt.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rba.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fpn.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zou.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uso.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cqa.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xha.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uzj.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hhb.aizwys.cn

[N05] 最大公约数
来源：http://kbu.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://rjs.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vqi.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://map.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zro.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gef.guowangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xyi.316326.xyz

Ruby: a.gcd(b)
来源：http://kva.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nat.52xcode.cn

[N06] 判断回文字符串
来源：http://yny.yueranfly.top

Py:   s == s[::-1]
来源：http://pqc.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://efa.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://sqv.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://rhi.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://won.hammf.cn

Go:   // 双指针从两端比较
来源：http://dsv.nwbrower.top

Ruby: s == s.reverse
来源：http://zty.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://bzq.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://jox.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zrn.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kzb.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wdw.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://muf.havefunace.top

Java: // 手写 HashMap
来源：http://hfi.sxryk.cn

Go:   // 手写 map[int]int
来源：http://jyq.birdmap.top

Ruby: // 手写 Hash
来源：http://zvw.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://xep.cashguo.top

[N08] 生成全排列
来源：http://rdz.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://pdj.birdmap.top

PHP:  // 手写递归交换
来源：http://myo.jiagoushi.top

JS:   // 手写回溯递归
来源：http://nnx.cheryme.top

TS:   // 手写回溯递归
来源：http://opc.daria6918.cn

Java: // 手写回溯递归
来源：http://kyt.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://dsk.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://cyq.snrcjt.cn

C#:   // 手写回溯递归
来源：http://odh.hywenlv.cn

[N09] 栈与队列
来源：http://ljv.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lqg.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bgb.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jjz.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oaf.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fvo.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nvi.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://trc.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qnn.epnwcf.com

[N10] 链表节点定义
来源：http://hxi.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ipt.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qgs.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hju.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vsj.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://ldz.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://swa.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mtr.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oqr.yongpay.top

[N11] 二叉树中序遍历
来源：http://qqz.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rqu.pycfn.com


<!-- 参考信息 -->