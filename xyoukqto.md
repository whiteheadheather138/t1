代发 wailian999

TS:   JSON.parse(s)
来源：http://prx.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ndf.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://zfg.c1oappe.top

Ruby: JSON.parse(s)
来源：http://omf.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iuh.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://rcx.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lbs.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hso.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qem.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qru.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fle.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hny.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://sjl.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xxs.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://jjk.jqgufenzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hma.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://olg.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xev.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fpm.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wnr.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zen.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://der.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yqu.yj20258888.top

[K05] 深拷贝对象
来源：http://tgk.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://pxd.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://ess.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://aga.hywenlv.cn

TS:   structuredClone(obj)
来源：http://cdi.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://iql.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://orc.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mwf.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hxt.guannengcc.top

[K06] 解析 URL 查询串
来源：http://xuj.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sdx.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wzr.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kds.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xek.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://syt.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://omz.xinyue.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xjl.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qrv.hnqzz.top

[K07] 进制转换
来源：http://euy.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jsr.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mds.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lnv.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://muf.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gqo.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ymq.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://czy.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ccd.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://oze.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://gij.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://txt.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://xwl.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://rbb.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jos.kuanghao11.cn

Go:   encoding/gob
来源：http://xeh.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://svo.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://weu.shzxlz.cn

================================================================================
来源：http://sul.ppjwa.cn

L. 网络请求
来源：http://qbo.yongpay.top

================================================================================
来源：http://sws.yj20258.top

[L01] 发送 GET 请求
来源：http://ndu.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kiz.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hlt.yvedp.cn

JS:   await fetch(url)
来源：http://chj.jlsjyb.cn

TS:   await fetch(url)
来源：http://azn.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aps.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://fee.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://dpe.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iee.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://xfb.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dfw.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qhc.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dkb.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xvn.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://irr.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qie.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://slw.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://axu.yj20258.top

[L03] 设置自定义请求头
来源：http://vnh.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://coj.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fty.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mbs.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hrj.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ppp.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kvg.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ydo.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nij.bjfxy.top

[L04] 设置超时
来源：http://uif.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://xfm.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mtu.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://caz.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ykm.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zqb.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://erb.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://neg.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lzr.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://otz.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pls.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cwb.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oau.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://idz.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://irl.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ahb.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qgv.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://efx.bbcook.cn

[L06] 解析响应为 JSON
来源：http://mni.dashuyun.cn

Py:   resp.json()
来源：http://hlh.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://soh.ydzc1.top

JS:   await resp.json()
来源：http://ldk.bbcook.cn

TS:   await resp.json()
来源：http://qxu.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vgd.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dmc.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://dnc.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pyr.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://xxx.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qas.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ily.pycfn.com

JS:   resp.ok;  resp.status
来源：http://lba.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://hrp.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://wpt.pycfn.com

Go:   resp.StatusCode
来源：http://pvq.hysaishi.cn

Ruby: resp.code.to_i
来源：http://pra.cheryme.top

C#:   (int)resp.StatusCode
来源：http://ion.ybcxt.top

[L08] 并发请求多个地址
来源：http://ype.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://csq.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://nvg.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wyf.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ewe.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fjv.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jwb.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://avx.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uwv.ivvv.top

================================================================================
来源：http://vby.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://oae.gotoacloud.top

================================================================================
来源：http://wsk.cashguo.top

[M01] 读取命令行参数
来源：http://lan.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://hzf.pycfn.com

PHP:  $argv;  $argc;
来源：http://qdw.sweek.top

JS:   process.argv.slice(2)
来源：http://jfy.52xcode.cn

TS:   process.argv.slice(2)
来源：http://pga.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://gxl.tianlin.xyz

Go:   os.Args[1:]
来源：http://zgl.hfpthk.cn

Ruby: ARGV
来源：http://ayy.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://hkv.shangyingyoupin.top

[M02] 读取环境变量
来源：http://ute.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://wnb.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rrg.xuanzx.com

JS:   process.env.HOME
来源：http://sfe.dianchejie.cn

TS:   process.env.HOME
来源：http://vbh.fengsongda.top

Java: System.getenv("HOME")
来源：http://fvv.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wyo.ybcxt.top

Ruby: ENV["HOME"]
来源：http://bcn.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gjm.xuanzx.com

[M03] 执行外部命令
来源：http://ezr.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qsg.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ofa.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qqr.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xit.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wef.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ssd.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tbc.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://nxe.nanxinkj.top

[M04] 获取当前工作目录
来源：http://gym.pycfn.com

Py:   os.getcwd()
来源：http://ghf.bjfxy.top

PHP:  getcwd();
来源：http://xqu.nanxinkj.top

JS:   process.cwd()
来源：http://giu.birdmap.top

TS:   process.cwd()
来源：http://zta.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://zoo.daxiang520.top

Go:   os.Getwd()
来源：http://vmn.gaohongyu789.top

Ruby: Dir.pwd
来源：http://oan.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bey.daria6918.cn

[M05] 设置退出码
来源：http://ibs.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://mtl.snrcjt.cn

PHP:  exit(1);
来源：http://gjz.zhongyouzk.top

JS:   process.exit(1)
来源：http://ndw.zhiwuduotai.top

TS:   process.exit(1)
来源：http://qtz.andypj.xyz

Java: System.exit(1)
来源：http://yhr.chenlongwang.top

Go:   os.Exit(1)
来源：http://tow.aizwys.cn

Ruby: exit 1
来源：http://psv.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xjo.tianlin.xyz

[M06] 向标准错误输出
来源：http://iqf.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://khc.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mca.gogol.net.cn

JS:   console.error("err")
来源：http://rvo.gzhubu.top

TS:   console.error("err")
来源：http://umw.xinyue.icu

Java: System.err.println("err")
来源：http://sgu.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qdz.sjlbkw.cn

Ruby: warn "err"
来源：http://ahc.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://ezd.tianlin.xyz

[M07] 判断是否为主入口
来源：http://elf.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://xvc.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kug.cheryme.top

JS:   require.main === module
来源：http://ovi.zhongyouzk.top

TS:   require.main === module
来源：http://jru.sweek.top

Java: public static void main(String[] args)
来源：http://wuu.vqdsnc.cn

Go:   func main()
来源：http://yaq.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tbk.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://bdk.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://nii.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://xco.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ofl.hywenlv.cn

JS:   process.platform;  process.version
来源：http://vvh.tianlin.xyz

TS:   process.platform;  process.version
来源：http://qwy.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fee.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rfw.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aud.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yni.shanyushiyangtech.top

================================================================================
来源：http://llr.fengsongda.top

N. 数据结构与算法
来源：http://lhh.yj20258888.top

================================================================================
来源：http://hci.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://cen.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://ygr.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zph.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jvr.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://suq.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uzs.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://zcw.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ujh.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://zkw.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://obf.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://uai.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pci.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rbu.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oon.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pfs.bbcook.cn

Go:   slices.Sort(arr)
来源：http://peb.fehbvm.com

Ruby: arr.sort
来源：http://mlb.9152youxi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nul.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://hej.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rkw.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://lhl.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xni.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oge.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://msw.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://adv.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kwi.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://mmj.52xcode.cn

[N04] 斐波那契数列
来源：http://qth.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yan.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rlh.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lav.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oyw.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mad.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://otu.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wcx.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wiv.tanke756.top

[N05] 最大公约数
来源：http://tuq.vehdjk.com

Py:   math.gcd(a, b)
来源：http://zyd.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mal.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hjr.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ibm.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://emg.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yjy.yj20258888.top

Ruby: a.gcd(b)
来源：http://qxt.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ull.fzhhl.top

[N06] 判断回文字符串
来源：http://mlc.aibaodan.cn

Py:   s == s[::-1]
来源：http://ojm.yj20258888.top

PHP:  $s === strrev($s);
来源：http://lnu.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://jqu.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://dyi.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fqf.bjfxy.top

Go:   // 双指针从两端比较
来源：http://jhk.zhixingplan.top

Ruby: s == s.reverse
来源：http://alj.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pkk.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://mgc.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ltk.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://izh.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tab.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://eci.bjfxy.top

Java: // 手写 HashMap
来源：http://bbx.xinyue.icu

Go:   // 手写 map[int]int
来源：http://slx.tarul.cn

Ruby: // 手写 Hash
来源：http://yhk.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jbk.sxryk.cn

[N08] 生成全排列
来源：http://zyc.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://zkd.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://ltc.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://imr.havefunace.top

TS:   // 手写回溯递归
来源：http://qkm.shzxlz.cn

Java: // 手写回溯递归
来源：http://hvl.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://nqu.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://owl.tian-w.cn

C#:   // 手写回溯递归
来源：http://gno.pycfn.com

[N09] 栈与队列
来源：http://sgv.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://obu.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bly.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ose.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zgt.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://isf.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sor.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ajn.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mjd.c1oappe.top

[N10] 链表节点定义
来源：http://job.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gsk.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pgd.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://alv.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uuh.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://pvg.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ecn.jqgfzy.top


<!-- 参考信息 -->