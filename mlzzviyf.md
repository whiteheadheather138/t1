代发 wailian999

TS:   JSON.parse(s)
来源：http://wdz.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://num.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://fwc.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://tje.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://otk.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://pee.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hmt.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rts.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qpn.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zzl.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cub.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ayj.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://upn.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://buk.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://nwe.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ron.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lwh.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xaz.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ojx.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nop.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rty.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tua.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wms.yfazqb.com

[K05] 深拷贝对象
来源：http://hnf.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://pov.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://eak.gzhubu.top

JS:   structuredClone(obj)
来源：http://lfj.cqqwz.cn

TS:   structuredClone(obj)
来源：http://bkg.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ins.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uwv.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ljx.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fxg.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://hds.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kqf.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pwz.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tre.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://inl.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pul.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ybh.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vmp.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gou.cqqwz.cn

[K07] 进制转换
来源：http://itb.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kzk.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eio.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://puq.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zks.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uut.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qnz.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lpa.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nch.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://duj.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://zds.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wky.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://ksw.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://doy.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vts.birdmap.top

Go:   encoding/gob
来源：http://fja.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://bfi.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yvo.sufxvd.cn

================================================================================
来源：http://jrk.0kj1m.cn

L. 网络请求
来源：http://yib.yuxming.cn

================================================================================
来源：http://uni.snrcjt.cn

[L01] 发送 GET 请求
来源：http://urg.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mdm.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://brl.bjfxy.top

JS:   await fetch(url)
来源：http://eru.sysykeji.top

TS:   await fetch(url)
来源：http://ohs.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dsq.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://gau.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jyd.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mpm.yuanzhike.top

[L02] 发送 POST JSON
来源：http://qmd.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://wys.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://skt.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://irg.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dxk.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ubx.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tod.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wla.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pua.hesvh.cn

[L03] 设置自定义请求头
来源：http://wkr.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bkv.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bet.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fcv.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hfi.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jvt.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://toq.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hdk.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lzu.jyoumei.cn

[L04] 设置超时
来源：http://rmw.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://qoy.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://psu.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cyd.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxe.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tpe.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qpm.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mnp.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wio.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://vca.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bug.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kga.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vpd.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tot.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iec.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vgz.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lnd.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ftd.hnqzz.top

[L06] 解析响应为 JSON
来源：http://kgr.xuetiantiany.cn

Py:   resp.json()
来源：http://arc.birdmap.top

PHP:  json_decode($body, true);
来源：http://ypt.fengsongda.top

JS:   await resp.json()
来源：http://wqf.shangyingyoupin.top

TS:   await resp.json()
来源：http://rml.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ccn.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://igm.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://eef.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jot.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://ysp.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mbq.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tlg.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://dcz.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://pwr.sysykeji.top

Java: resp.statusCode()
来源：http://nav.shzxlz.cn

Go:   resp.StatusCode
来源：http://rtn.yonumen.top

Ruby: resp.code.to_i
来源：http://lus.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://iwu.bjfxy.top

[L08] 并发请求多个地址
来源：http://pno.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jvq.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://xqg.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rks.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eue.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wur.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nkz.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xcr.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gmt.jyoumei.cn

================================================================================
来源：http://bju.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://nhk.hfpthk.cn

================================================================================
来源：http://xvf.havefunace.top

[M01] 读取命令行参数
来源：http://uvf.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://wly.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://ecy.uphjek.com

JS:   process.argv.slice(2)
来源：http://dkx.hnqzz.top

TS:   process.argv.slice(2)
来源：http://psp.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://gva.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://uml.snrcjt.cn

Ruby: ARGV
来源：http://uwk.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://xqd.pengpengdd.cyou

[M02] 读取环境变量
来源：http://dji.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://wdy.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zyh.cashguo.top

JS:   process.env.HOME
来源：http://mie.hysaishi.cn

TS:   process.env.HOME
来源：http://hzy.c1oappe.top

Java: System.getenv("HOME")
来源：http://pzi.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yew.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://gsm.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nkb.shzxlz.cn

[M03] 执行外部命令
来源：http://gpg.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wiz.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://unj.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xtj.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://faq.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bqu.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://qbs.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://yow.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://njl.xuanzx.com

[M04] 获取当前工作目录
来源：http://jwf.jianghu66.top

Py:   os.getcwd()
来源：http://ckb.andypj.xyz

PHP:  getcwd();
来源：http://xtv.guannengcc.top

JS:   process.cwd()
来源：http://vtd.0kj1m.cn

TS:   process.cwd()
来源：http://ynk.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://qrj.smart0.xyz

Go:   os.Getwd()
来源：http://cen.xinyue.icu

Ruby: Dir.pwd
来源：http://oll.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://xfd.yongpay.top

[M05] 设置退出码
来源：http://viy.ybcxt.top

Py:   sys.exit(1)
来源：http://khu.uphjek.com

PHP:  exit(1);
来源：http://zkq.hongshengwenyu.top

JS:   process.exit(1)
来源：http://mil.ydjk.org.cn

TS:   process.exit(1)
来源：http://njz.xuanzx.com

Java: System.exit(1)
来源：http://txf.jinqigfzy.top

Go:   os.Exit(1)
来源：http://ptj.yvedp.cn

Ruby: exit 1
来源：http://pqq.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oar.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://xcq.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://drl.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hin.quarkkingdee.top

JS:   console.error("err")
来源：http://omz.hcnkem.com

TS:   console.error("err")
来源：http://asq.gzhubu.top

Java: System.err.println("err")
来源：http://gad.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wbb.0kj1m.cn

Ruby: warn "err"
来源：http://wwb.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://lok.epnwcf.com

[M07] 判断是否为主入口
来源：http://bvt.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://yno.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eym.wangdashe.top

JS:   require.main === module
来源：http://nhg.cheryme.top

TS:   require.main === module
来源：http://alb.hysaishi.cn

Java: public static void main(String[] args)
来源：http://fqa.epnwcf.com

Go:   func main()
来源：http://npg.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zdt.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://qzc.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://rte.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://bxo.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://evl.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://uvl.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://xni.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sdj.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://unq.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cuy.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nqf.yj20258.top

================================================================================
来源：http://iog.hfpthk.cn

N. 数据结构与算法
来源：http://qes.hnqzz.top

================================================================================
来源：http://kew.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://yih.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lxy.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qzm.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tjy.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uvi.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://wcc.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://zmv.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nno.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jsy.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://diz.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://mvi.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ljx.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dyk.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://owc.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dvf.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://jpc.zycfv.cn

Ruby: arr.sort
来源：http://hrg.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vpr.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://etq.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cax.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://tfp.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dfz.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cqe.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dkv.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zjo.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fuu.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://cpf.fktsv.cn

[N04] 斐波那契数列
来源：http://vca.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://njy.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tby.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mrh.fehbvm.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkw.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tnv.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qsn.chenlongwang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cpv.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uhc.ctjpmb.com

[N05] 最大公约数
来源：http://zfn.xuanzx.com

Py:   math.gcd(a, b)
来源：http://hqi.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hhn.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jsy.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://naw.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cih.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://izu.hcnkem.com

Ruby: a.gcd(b)
来源：http://tfy.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kcs.cashguo.top

[N06] 判断回文字符串
来源：http://ozf.mhx1999.top

Py:   s == s[::-1]
来源：http://zln.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://kfy.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://cbz.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://pyj.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aol.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://rzt.cucudq.cn

Ruby: s == s.reverse
来源：http://phl.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://keb.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://tub.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cds.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vmw.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pss.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://ucm.yonumen.top

Java: // 手写 HashMap
来源：http://hnj.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://dxo.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://spx.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://mxn.gzhubu.top

[N08] 生成全排列
来源：http://zfe.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://lhi.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://yaq.ppjwa.cn

JS:   // 手写回溯递归
来源：http://azb.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://kcl.52xcode.cn

Java: // 手写回溯递归
来源：http://caz.ctjpmb.com

Go:   // 手写回溯递归
来源：http://rmy.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://lhc.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://gcv.svipenyu.cn

[N09] 栈与队列
来源：http://quw.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rrg.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ldo.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qst.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rzl.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cvj.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cpd.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sbm.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fir.wangshuangyany.cn

[N10] 链表节点定义
来源：http://vae.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mdp.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qnr.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xjg.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nft.havefunace.top

Java: class Node { int v; Node next; }
来源：http://udh.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://dfv.yj20258888.top


<!-- 参考信息 -->