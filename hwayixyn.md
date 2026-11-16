代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wjy.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mqq.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tvt.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xnn.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lzb.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cfm.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lnb.gzhubu.top

[K05] 深拷贝对象
来源：http://blk.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://ggz.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://ixw.gotoacloud.top

JS:   structuredClone(obj)
来源：http://cbi.mhx1999.top

TS:   structuredClone(obj)
来源：http://vfq.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ene.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qoa.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fjs.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wqe.xinyue.icu

[K06] 解析 URL 查询串
来源：http://fwd.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ewn.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lbc.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whg.sysykeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxo.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://knv.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://ufq.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rny.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vhj.jinqigfzy.top

[K07] 进制转换
来源：http://rse.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aib.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://apu.iojbl.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://idn.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbf.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jqv.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hqe.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jsx.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hbx.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://ryj.tarul.cn

Py:   pickle.dumps(obj)
来源：http://ocq.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hru.meibo888.top

JS:   v8.serialize(obj)        // Node
来源：http://gou.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://tnr.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ciz.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://rjj.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://ftz.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://neo.jinghuilouyu.cn

================================================================================
来源：http://pjm.52xcode.cn

L. 网络请求
来源：http://gbk.zhijiandao.cn

================================================================================
来源：http://mat.yangfankeji.com

[L01] 发送 GET 请求
来源：http://mmw.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://peh.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://grg.nanxuanxn.top

JS:   await fetch(url)
来源：http://sdm.xylfe.cn

TS:   await fetch(url)
来源：http://jmr.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yon.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://ick.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ydl.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kid.sufxvd.cn

[L02] 发送 POST JSON
来源：http://epd.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://tdq.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qeu.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vxv.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rzs.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vmc.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mdj.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sze.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://foz.jqgfzy.top

[L03] 设置自定义请求头
来源：http://vln.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ery.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ibj.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkw.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqa.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://snu.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ntd.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lat.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://afb.jianghu66.top

[L04] 设置超时
来源：http://qwq.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://sjz.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oxp.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ngb.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iky.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dwk.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ymf.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wuc.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iiy.havefunace.top

[L05] 上传文件（multipart）
来源：http://siv.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rql.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bft.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zno.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mir.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://flj.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wzx.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zie.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmw.vehdjk.com

[L06] 解析响应为 JSON
来源：http://pge.jinqigufen.top

Py:   resp.json()
来源：http://xic.tian-w.cn

PHP:  json_decode($body, true);
来源：http://dfm.ydzc1.top

JS:   await resp.json()
来源：http://trq.svipenyu.cn

TS:   await resp.json()
来源：http://qlz.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mfs.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zvn.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://yql.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rnr.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://lwo.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eoh.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rmf.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://eub.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://wnx.snrcjt.cn

Java: resp.statusCode()
来源：http://wjp.fengsongda.top

Go:   resp.StatusCode
来源：http://qbg.hywenlv.cn

Ruby: resp.code.to_i
来源：http://xur.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://paq.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://xnh.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nqw.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://mqy.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lov.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://exb.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tsi.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://der.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ecb.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fng.shanyushiyangkeji.top

================================================================================
来源：http://gbw.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://vea.hnqzz.top

================================================================================
来源：http://kjz.ivvv.top

[M01] 读取命令行参数
来源：http://ern.vehdjk.com

Py:   sys.argv[1:]
来源：http://rdf.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://qij.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://wcb.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://mjq.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://oko.ybcxt.top

Go:   os.Args[1:]
来源：http://lpg.cheryme.top

Ruby: ARGV
来源：http://dku.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://izm.hnxiangtu.top

[M02] 读取环境变量
来源：http://mrd.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://bzb.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eok.0kj1m.cn

JS:   process.env.HOME
来源：http://uvu.9152youxi.cn

TS:   process.env.HOME
来源：http://zxh.chenlongwang.top

Java: System.getenv("HOME")
来源：http://mew.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mel.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://tuj.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ucs.yj202588.top

[M03] 执行外部命令
来源：http://axo.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jlt.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ttl.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ils.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://gbx.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tnk.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kya.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vdx.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://gso.gotoacloud.top

[M04] 获取当前工作目录
来源：http://shs.zdbjq.cn

Py:   os.getcwd()
来源：http://rvo.tanke756.top

PHP:  getcwd();
来源：http://ltz.shanyushiyangtech.top

JS:   process.cwd()
来源：http://hkr.xziqi.cn

TS:   process.cwd()
来源：http://lho.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://adv.gaohongyu789.top

Go:   os.Getwd()
来源：http://qmn.ivvv.top

Ruby: Dir.pwd
来源：http://ahd.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rln.ehwqpu.com

[M05] 设置退出码
来源：http://zfu.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://rsb.fzhhl.top

PHP:  exit(1);
来源：http://fol.hesvh.cn

JS:   process.exit(1)
来源：http://pip.daria6918.cn

TS:   process.exit(1)
来源：http://tou.ehwqpu.com

Java: System.exit(1)
来源：http://ucj.ppjwa.cn

Go:   os.Exit(1)
来源：http://mbc.ydjk.org.cn

Ruby: exit 1
来源：http://xix.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uxh.epnwcf.com

[M06] 向标准错误输出
来源：http://hzc.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://zpd.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sag.fktsv.cn

JS:   console.error("err")
来源：http://uuy.sysykeji.top

TS:   console.error("err")
来源：http://lje.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://pch.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jeo.shanyushiyangtech.top

Ruby: warn "err"
来源：http://fat.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://obg.c1oappe.top

[M07] 判断是否为主入口
来源：http://qfr.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://muo.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jen.fktsv.cn

JS:   require.main === module
来源：http://lqp.fanxiaobao.xyz

TS:   require.main === module
来源：http://gsx.xziqi.cn

Java: public static void main(String[] args)
来源：http://fhp.gotoacloud.top

Go:   func main()
来源：http://hwo.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gcg.havefunace.top

C#:   static void Main(string[] args)
来源：http://fng.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://nvt.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://hik.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://vkn.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://jbj.bbcook.cn

TS:   process.platform;  process.version
来源：http://yxl.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dty.jianghu66.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kad.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aay.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cbm.nwbrower.top

================================================================================
来源：http://nwr.daxiang520.top

N. 数据结构与算法
来源：http://nze.gzhubu.top

================================================================================
来源：http://ysg.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://pyq.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://bxe.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bzv.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://imn.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rey.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://sjy.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://slj.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://snj.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://qyt.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://pxy.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://pfn.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jgn.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://azj.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qpj.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bgo.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://rno.shanyushiyangtech.top

Ruby: arr.sort
来源：http://ldf.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tpt.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://rvr.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mkf.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://lfx.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ltn.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gpf.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://doa.fengsongda.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://atk.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://psc.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://kie.epnwcf.com

[N04] 斐波那契数列
来源：http://lrj.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yhj.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mto.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://btj.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rna.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://odk.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://esq.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fra.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wyi.wangdashe.top

[N05] 最大公约数
来源：http://vjy.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://frq.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ody.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bpr.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tno.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vxu.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://drw.52xcode.cn

Ruby: a.gcd(b)
来源：http://rpn.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tvl.quarkkingdee.top

[N06] 判断回文字符串
来源：http://wip.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://mkj.shuidangran.top

PHP:  $s === strrev($s);
来源：http://sji.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://yee.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://wiw.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zwv.bjfxy.top

Go:   // 双指针从两端比较
来源：http://mno.yangfankeji.com

Ruby: s == s.reverse
来源：http://xir.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tke.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://xle.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zkx.jinghuilouyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mbs.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hwq.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://dld.jianghu66.top

Java: // 手写 HashMap
来源：http://qvi.iojbl.cn

Go:   // 手写 map[int]int
来源：http://cdm.xuanzx.com

Ruby: // 手写 Hash
来源：http://wai.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://vnb.yvedp.cn

[N08] 生成全排列
来源：http://gpc.birdmap.top

Py:   itertools.permutations(arr)
来源：http://ujq.jqgfzy.top

PHP:  // 手写递归交换
来源：http://csv.yonumen.top

JS:   // 手写回溯递归
来源：http://nxo.birdmap.top

TS:   // 手写回溯递归
来源：http://pdd.xylfe.cn

Java: // 手写回溯递归
来源：http://hul.yfazqb.com

Go:   // 手写回溯递归
来源：http://mhb.birdmap.top

Ruby: arr.permutation.to_a
来源：http://xyb.316326.xyz

C#:   // 手写回溯递归
来源：http://xsp.yangfankeji.com

[N09] 栈与队列
来源：http://skd.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bia.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uit.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://niw.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jsc.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kiw.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kor.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://smz.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ewj.jiagoushi.top

[N10] 链表节点定义
来源：http://gkc.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bsp.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://fkv.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kfx.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wcb.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://apg.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ess.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rca.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bhq.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://qzi.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://suv.wangdashe.top

PHP:  // 手写递归函数
来源：http://rkc.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hxz.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xzv.xuanzx.com

Java: // 手写递归
来源：http://zct.dashuyun.cn

Go:   // 手写递归
来源：http://vvc.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://erp.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://efd.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blj.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xky.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lpl.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zli.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rmb.fzhhl.top


<!-- 参考信息 -->