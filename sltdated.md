代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://amu.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sfk.guannengcc.top

[K04] 读取 JSON 文件
来源：http://tsg.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xup.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iqq.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ixk.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://txd.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://izj.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qrx.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wrj.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://smr.dashuyun.cn

[K05] 深拷贝对象
来源：http://arc.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://kuc.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://atg.wangdashe.top

JS:   structuredClone(obj)
来源：http://oyk.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://rmb.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://twy.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://phk.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uur.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gup.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://rfg.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gca.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vhm.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kng.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pik.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://phs.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tov.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pjw.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gqd.yonumen.top

[K07] 进制转换
来源：http://ltn.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oxj.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ola.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sss.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mbd.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mtl.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bgb.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lkw.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://elx.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://kgt.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://ths.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://cgw.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://soe.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://mys.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fux.shzxlz.cn

Go:   encoding/gob
来源：http://eqy.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://gto.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tfj.gaohongyu789.top

================================================================================
来源：http://wsl.wangdashe.top

L. 网络请求
来源：http://rmu.xuanzx.com

================================================================================
来源：http://tcg.cheryme.top

[L01] 发送 GET 请求
来源：http://ubm.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gsz.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://atd.hesvh.cn

JS:   await fetch(url)
来源：http://zzx.fzhhl.top

TS:   await fetch(url)
来源：http://dgk.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uzn.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://xvy.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vtt.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://unv.yfazqb.com

[L02] 发送 POST JSON
来源：http://xnn.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://hgg.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xzt.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xzz.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wpb.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gba.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yyb.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wao.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bwf.tanke756.top

[L03] 设置自定义请求头
来源：http://olv.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jaa.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rte.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://htj.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vct.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://unb.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mdu.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qym.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://whb.cqqwz.cn

[L04] 设置超时
来源：http://toa.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://kau.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dbg.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iwp.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oii.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mlk.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uwc.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qie.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ynn.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://wmy.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qhf.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ikd.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wlt.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cph.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pnp.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tgu.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nuz.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kvj.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://rpc.316326.xyz

Py:   resp.json()
来源：http://wbu.bjfxy.top

PHP:  json_decode($body, true);
来源：http://zdf.jyoumei.cn

JS:   await resp.json()
来源：http://cvc.zhengqikj.top

TS:   await resp.json()
来源：http://ioc.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://liu.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vps.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://rwj.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ddu.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://koq.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vzo.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dvg.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://zlx.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://xvx.ehwqpu.com

Java: resp.statusCode()
来源：http://zpd.vehdjk.com

Go:   resp.StatusCode
来源：http://jvh.xziqi.cn

Ruby: resp.code.to_i
来源：http://qkg.ivvv.top

C#:   (int)resp.StatusCode
来源：http://mhj.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://qng.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xmz.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://qst.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wvk.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://isn.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cxz.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lez.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://for.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ygc.bjfxy.top

================================================================================
来源：http://qrg.tianlin.xyz

M. 命令行 / 进程 / 环境
来源：http://egy.chenjidiqi.icu

================================================================================
来源：http://lme.yfazqb.com

[M01] 读取命令行参数
来源：http://thz.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://nud.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://cfv.bjfxy.top

JS:   process.argv.slice(2)
来源：http://nbf.cucudq.cn

TS:   process.argv.slice(2)
来源：http://fho.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://wxq.dashuyun.cn

Go:   os.Args[1:]
来源：http://fjc.gaohongyu789.top

Ruby: ARGV
来源：http://kgf.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://eqj.havefunace.top

[M02] 读取环境变量
来源：http://pcn.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://xqf.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://itm.quarkkingdee.top

JS:   process.env.HOME
来源：http://ptx.ydjk.org.cn

TS:   process.env.HOME
来源：http://hjp.andypj.xyz

Java: System.getenv("HOME")
来源：http://tmq.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ozb.ivvv.top

Ruby: ENV["HOME"]
来源：http://lob.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bmw.jinqigfzy.top

[M03] 执行外部命令
来源：http://fnv.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cje.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pfb.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://edx.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jdt.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ioj.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://jlr.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://vbe.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://vcy.jyoumei.cn

[M04] 获取当前工作目录
来源：http://rno.feifeiyinyue.top

Py:   os.getcwd()
来源：http://tmu.52xcode.cn

PHP:  getcwd();
来源：http://tfs.cheryme.top

JS:   process.cwd()
来源：http://kyd.fktsv.cn

TS:   process.cwd()
来源：http://etw.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://vlg.nwbrower.top

Go:   os.Getwd()
来源：http://tdc.fengsongda.top

Ruby: Dir.pwd
来源：http://ecy.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://isq.xuetiantiany.cn

[M05] 设置退出码
来源：http://uem.jinqigufen.top

Py:   sys.exit(1)
来源：http://izc.guowangkeji.top

PHP:  exit(1);
来源：http://bkt.9152youxi.cn

JS:   process.exit(1)
来源：http://ugf.zdbjq.cn

TS:   process.exit(1)
来源：http://twh.jianghu66.top

Java: System.exit(1)
来源：http://igb.9152youxi.cn

Go:   os.Exit(1)
来源：http://fqt.tanke756.top

Ruby: exit 1
来源：http://dlr.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ewy.cqqwz.cn

[M06] 向标准错误输出
来源：http://via.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://yqy.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://poz.ydjk.org.cn

JS:   console.error("err")
来源：http://weu.svipenyu.cn

TS:   console.error("err")
来源：http://uwv.hammf.cn

Java: System.err.println("err")
来源：http://jfu.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://txe.ehwqpu.com

Ruby: warn "err"
来源：http://pvr.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://cxk.svipenyu.cn

[M07] 判断是否为主入口
来源：http://dpw.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://cll.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dyq.zdqjudy.top

JS:   require.main === module
来源：http://lsb.xinyue.icu

TS:   require.main === module
来源：http://avx.epnwcf.com

Java: public static void main(String[] args)
来源：http://ksh.ydzc1.top

Go:   func main()
来源：http://qbf.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rgk.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://lrl.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://kcu.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://wkx.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://mwb.uphjek.com

JS:   process.platform;  process.version
来源：http://poc.xuanzx.com

TS:   process.platform;  process.version
来源：http://kbt.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://any.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://aup.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ruo.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lzb.nanxinkj.top

================================================================================
来源：http://qeg.guowangkeji.top

N. 数据结构与算法
来源：http://qzg.jinqigufen.top

================================================================================
来源：http://owi.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://bqh.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://jdh.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pph.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rdj.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knz.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://drz.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://xqw.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ali.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://pyl.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://lgo.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://bma.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ziq.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lak.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kcj.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jzh.yonumen.top

Go:   slices.Sort(arr)
来源：http://hun.snrcjt.cn

Ruby: arr.sort
来源：http://fsn.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://byu.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://pzh.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://weo.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://wyb.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lft.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jkv.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ngl.sjlbkw.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://emm.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nuj.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bde.chenlongwang.top

[N04] 斐波那契数列
来源：http://dfz.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ktt.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uhi.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zzo.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xap.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rsk.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qvf.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ogo.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rhq.hammf.cn

[N05] 最大公约数
来源：http://cpu.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://djo.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vuu.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://utf.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pei.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bwn.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nxh.cucudq.cn

Ruby: a.gcd(b)
来源：http://whr.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ttr.vqdsnc.cn

[N06] 判断回文字符串
来源：http://thm.nanxuanxn.top

Py:   s == s[::-1]
来源：http://bwg.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://aiw.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://zrv.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://jby.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tar.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://bvq.hnqzz.top

Ruby: s == s.reverse
来源：http://yan.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://iqc.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://ehr.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://auz.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fnn.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qca.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://bwd.tianlin.xyz

Java: // 手写 HashMap
来源：http://ytj.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://ujq.xinyue.icu

Ruby: // 手写 Hash
来源：http://zvu.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://ysm.xinyue.icu

[N08] 生成全排列
来源：http://mgq.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://wyh.yj20258.top

PHP:  // 手写递归交换
来源：http://srs.guannengcc.top

JS:   // 手写回溯递归
来源：http://yvt.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://xnh.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://gfs.yvedp.cn

Go:   // 手写回溯递归
来源：http://iro.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://mke.cheryme.top

C#:   // 手写回溯递归
来源：http://thd.jianghu66.top

[N09] 栈与队列
来源：http://zyb.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://loi.wangshuangyany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://enz.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qgs.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aqi.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oft.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xmn.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qir.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hiu.meibo888.top

[N10] 链表节点定义
来源：http://tbs.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pax.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dxa.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://duy.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://odp.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://ipt.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://myk.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yed.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://axh.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://oeu.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kjb.hammf.cn

PHP:  // 手写递归函数
来源：http://wzj.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lyw.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tiv.hcnkem.com

Java: // 手写递归
来源：http://saw.jqgufenzy.top

Go:   // 手写递归
来源：http://hqn.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yjy.yonumen.top

C#:   // 手写递归
来源：http://dij.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://idt.yanxiufei.cn


<!-- 参考信息 -->