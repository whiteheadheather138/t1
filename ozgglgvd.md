代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://bfw.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rnl.sysykeji.top

[K04] 读取 JSON 文件
来源：http://glr.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yco.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ijn.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ump.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://elf.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cob.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://las.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jlo.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qxg.yj20258.top

[K05] 深拷贝对象
来源：http://hth.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://pby.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://rli.guowangkeji.top

JS:   structuredClone(obj)
来源：http://grl.vehdjk.com

TS:   structuredClone(obj)
来源：http://nnz.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nov.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://svm.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jni.kuanghao11.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kir.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://qig.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ees.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ebc.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://osl.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bgm.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dkt.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://rhy.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lby.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ocq.jinghuilouyu.cn

[K07] 进制转换
来源：http://chn.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dkv.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://swg.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xmx.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sag.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dsv.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fsp.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kbz.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jfp.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://dds.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://dpf.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://abi.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://pcq.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://zxr.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://znb.wangshuangyany.cn

Go:   encoding/gob
来源：http://hmy.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://cpn.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mcn.tian-w.cn

================================================================================
来源：http://pca.sysykeji.top

L. 网络请求
来源：http://vbz.kuanghao11.cn

================================================================================
来源：http://pkk.cqqwz.cn

[L01] 发送 GET 请求
来源：http://zuj.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ehz.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://npp.shzxlz.cn

JS:   await fetch(url)
来源：http://wgs.hongshengwenyu.top

TS:   await fetch(url)
来源：http://jim.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gsg.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://pyx.kuanghao11.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cgt.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bzj.xziqi.cn

[L02] 发送 POST JSON
来源：http://pui.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gvr.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eyz.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wfz.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gms.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://epm.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uvx.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gby.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iov.fktsv.cn

[L03] 设置自定义请求头
来源：http://zdo.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pmw.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qrp.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yiy.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zyb.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lhl.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kqv.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rcx.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vtn.uphjek.com

[L04] 设置超时
来源：http://ooi.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://ovq.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://llo.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vbf.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lxi.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tlo.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ifg.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zkg.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://djj.ivvv.top

[L05] 上传文件（multipart）
来源：http://lyu.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hab.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vgv.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lia.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://arj.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zwa.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jbb.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ipe.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://san.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://ula.hysaishi.cn

Py:   resp.json()
来源：http://xwd.vehdjk.com

PHP:  json_decode($body, true);
来源：http://eco.sxryk.cn

JS:   await resp.json()
来源：http://vjx.bjfxy.top

TS:   await resp.json()
来源：http://wsy.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xrn.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ora.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://nvw.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xfs.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://woz.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pia.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mjs.meibo888.top

JS:   resp.ok;  resp.status
来源：http://pjb.yonumen.top

TS:   resp.ok;  resp.status
来源：http://kkd.fengsongda.top

Java: resp.statusCode()
来源：http://saf.tarul.cn

Go:   resp.StatusCode
来源：http://day.zycfv.cn

Ruby: resp.code.to_i
来源：http://fcs.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://drg.52xcode.cn

[L08] 并发请求多个地址
来源：http://tyk.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oin.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://seq.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wtp.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hre.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hoe.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qxi.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pbf.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mzn.redwolf501.top

================================================================================
来源：http://jjx.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://enl.ydzc1.top

================================================================================
来源：http://tbr.sxryk.cn

[M01] 读取命令行参数
来源：http://mpe.meibo888.top

Py:   sys.argv[1:]
来源：http://wiy.zycfv.cn

PHP:  $argv;  $argc;
来源：http://fdt.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://zdz.sweek.top

TS:   process.argv.slice(2)
来源：http://fyf.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://bkh.tarul.cn

Go:   os.Args[1:]
来源：http://xbv.xziqi.cn

Ruby: ARGV
来源：http://pub.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://saj.pengpengdd.cyou

[M02] 读取环境变量
来源：http://yfu.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://rpp.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fue.iojbl.cn

JS:   process.env.HOME
来源：http://mvs.hnqzz.top

TS:   process.env.HOME
来源：http://miw.zycfv.cn

Java: System.getenv("HOME")
来源：http://lno.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hdi.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://blx.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://adt.yvedp.cn

[M03] 执行外部命令
来源：http://nrr.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cul.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jir.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://gcf.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ybv.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wkd.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zwo.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bra.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://nwl.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://xza.cucudq.cn

Py:   os.getcwd()
来源：http://gfs.hywenlv.cn

PHP:  getcwd();
来源：http://jnm.quarkkingdee.top

JS:   process.cwd()
来源：http://tjf.ehwqpu.com

TS:   process.cwd()
来源：http://fni.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://htx.sxryk.cn

Go:   os.Getwd()
来源：http://cuq.yfazqb.com

Ruby: Dir.pwd
来源：http://vrd.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://cuk.zycfv.cn

[M05] 设置退出码
来源：http://drc.cheryme.top

Py:   sys.exit(1)
来源：http://fvs.fengsongda.top

PHP:  exit(1);
来源：http://trc.yongpay.top

JS:   process.exit(1)
来源：http://abx.nanxuanxn.top

TS:   process.exit(1)
来源：http://izh.xuetiantiany.cn

Java: System.exit(1)
来源：http://fdm.mhx1999.top

Go:   os.Exit(1)
来源：http://kyt.kuanghao11.cn

Ruby: exit 1
来源：http://gwa.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fbc.ivvv.top

[M06] 向标准错误输出
来源：http://qyv.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://lzf.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gfg.kuanghao11.cn

JS:   console.error("err")
来源：http://tzx.meibo888.top

TS:   console.error("err")
来源：http://zim.gaohongyu789.top

Java: System.err.println("err")
来源：http://nuk.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ozn.quarkkingdee.top

Ruby: warn "err"
来源：http://scj.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://rgm.yongpay.top

[M07] 判断是否为主入口
来源：http://suz.yj20258.top

Py:   if __name__ == "__main__":
来源：http://nxl.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://afi.snrcjt.cn

JS:   require.main === module
来源：http://dff.yonumen.top

TS:   require.main === module
来源：http://bsi.pycfn.com

Java: public static void main(String[] args)
来源：http://ins.aizwys.cn

Go:   func main()
来源：http://xdp.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jxn.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://hpo.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://eui.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://miw.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://esh.316326.xyz

JS:   process.platform;  process.version
来源：http://ytq.xuanzx.com

TS:   process.platform;  process.version
来源：http://oye.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qzp.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bpp.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kuf.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gsa.316326.xyz

================================================================================
来源：http://rlk.tarul.cn

N. 数据结构与算法
来源：http://oxi.ydzc1.top

================================================================================
来源：http://hok.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://nzn.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://liz.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yfd.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jye.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgo.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://odj.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://gak.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yem.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mtr.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://epw.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://vpn.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://frs.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://gxc.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kyb.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qsv.hammf.cn

Go:   slices.Sort(arr)
来源：http://sio.wangdashe.top

Ruby: arr.sort
来源：http://mwk.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://wdc.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://dnb.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://olp.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://tmc.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qws.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fjf.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zug.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wpn.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nsb.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rbk.gaohongyu789.top

[N04] 斐波那契数列
来源：http://xbm.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://apn.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://etm.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rpu.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ruk.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ime.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ysn.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sfx.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jvu.zhixingplan.top

[N05] 最大公约数
来源：http://cwu.xziqi.cn

Py:   math.gcd(a, b)
来源：http://ixv.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nqy.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gff.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrx.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jba.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gbn.sufxvd.cn

Ruby: a.gcd(b)
来源：http://pht.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sak.tianlin.xyz

[N06] 判断回文字符串
来源：http://tbl.zdqjudy.top

Py:   s == s[::-1]
来源：http://xrz.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://mrq.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://vug.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://zub.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bfh.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://yuv.zhengqikj.top

Ruby: s == s.reverse
来源：http://nds.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lbd.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://nwo.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cjz.dashuyun.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://abp.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uwd.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://gea.yonumen.top

Java: // 手写 HashMap
来源：http://iia.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://xgm.sufxvd.cn

Ruby: // 手写 Hash
来源：http://jyj.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://tuq.ivvv.top

[N08] 生成全排列
来源：http://vdl.hammf.cn

Py:   itertools.permutations(arr)
来源：http://vcw.zhengqikj.top

PHP:  // 手写递归交换
来源：http://nvq.yj20258888.top

JS:   // 手写回溯递归
来源：http://hsc.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://rax.yj20258888.top

Java: // 手写回溯递归
来源：http://bol.guannengcc.top

Go:   // 手写回溯递归
来源：http://fjt.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://ajk.xylfe.cn

C#:   // 手写回溯递归
来源：http://etp.hysaishi.cn

[N09] 栈与队列
来源：http://efo.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nwl.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bkr.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zwg.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://arz.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dbc.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://klg.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qkf.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ndp.ctjpmb.com

[N10] 链表节点定义
来源：http://dhm.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wah.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://koy.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iie.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ddx.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://cyj.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://zjf.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://mqu.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bcz.birdmap.top

[N11] 二叉树中序遍历
来源：http://qvt.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wfh.hesvh.cn

PHP:  // 手写递归函数
来源：http://mub.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjt.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qql.yj20258888.top

Java: // 手写递归
来源：http://zrk.zhongyouzk.top

Go:   // 手写递归
来源：http://rht.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gvl.jyoumei.cn

C#:   // 手写递归
来源：http://toa.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aij.fzhhl.top


<!-- 参考信息 -->