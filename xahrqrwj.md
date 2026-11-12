代发 wailian999

[K02] JSON 字符串转对象
来源：http://oso.shangyingyoupin.top

Py:   json.loads(s)
来源：http://fyu.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lqs.cqqwz.cn

JS:   JSON.parse(s)
来源：http://vpk.gotoacloud.top

TS:   JSON.parse(s)
来源：http://zke.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nyh.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://nou.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://zoh.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cjx.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://fes.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://otj.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://emj.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dgd.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cva.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qdq.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jmv.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://twt.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xfr.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://uka.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://efn.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hgz.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nxq.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhx.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bob.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tkd.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://gfv.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ktt.yangfankeji.com

[K05] 深拷贝对象
来源：http://krw.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://mae.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://baj.hfpthk.cn

JS:   structuredClone(obj)
来源：http://ctm.havefunace.top

TS:   structuredClone(obj)
来源：http://bsp.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bvb.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rvg.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://atf.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://lpn.smart0.xyz

[K06] 解析 URL 查询串
来源：http://hdy.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjz.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://npv.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://klm.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sql.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tux.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iwq.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tue.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cnt.epnwcf.com

[K07] 进制转换
来源：http://zar.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mnl.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jgb.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://omm.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nay.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ecm.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zxq.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oge.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xxo.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://qun.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://rgd.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://yib.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://rux.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://kyy.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ltp.xinyue.icu

Go:   encoding/gob
来源：http://nyw.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://djw.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://plq.svipenyu.cn

================================================================================
来源：http://mpl.jyoumei.cn

L. 网络请求
来源：http://kig.cashguo.top

================================================================================
来源：http://gpi.zdqjudy.top

[L01] 发送 GET 请求
来源：http://glw.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fod.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://clo.yuxming.cn

JS:   await fetch(url)
来源：http://xky.zhijiandao.cn

TS:   await fetch(url)
来源：http://rsj.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wca.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://usi.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tbo.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yik.yfazqb.com

[L02] 发送 POST JSON
来源：http://jgk.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ril.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lfq.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ngt.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hyd.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pys.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ikg.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hfu.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cgt.fktsv.cn

[L03] 设置自定义请求头
来源：http://wfz.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://abh.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dje.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://maq.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uua.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ubv.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zes.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hgz.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gdj.hammf.cn

[L04] 设置超时
来源：http://jvk.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://obg.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uwx.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gak.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aax.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qko.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ojz.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vzl.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sle.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://rep.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jxp.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uwg.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lqt.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://urt.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xbf.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dde.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://izl.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ycy.jinqigfzy.top

[L06] 解析响应为 JSON
来源：http://ydr.jinqigfzy.top

Py:   resp.json()
来源：http://rsi.yuxming.cn

PHP:  json_decode($body, true);
来源：http://txd.sufxvd.cn

JS:   await resp.json()
来源：http://wwt.yangfankeji.com

TS:   await resp.json()
来源：http://euz.ctjpmb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tnx.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://neg.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://yjn.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nxz.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://wls.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ggx.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oeh.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://bny.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://vqy.hnqzz.top

Java: resp.statusCode()
来源：http://puk.meibo888.top

Go:   resp.StatusCode
来源：http://dte.zdbjq.cn

Ruby: resp.code.to_i
来源：http://liw.birdmap.top

C#:   (int)resp.StatusCode
来源：http://afw.yangfankeji.com

[L08] 并发请求多个地址
来源：http://xca.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jzn.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://eek.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkl.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gve.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uot.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hts.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ura.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dvk.zhongyouzk.top

================================================================================
来源：http://gee.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://lyl.0kj1m.cn

================================================================================
来源：http://wir.hnqzz.top

[M01] 读取命令行参数
来源：http://sth.mhx1999.top

Py:   sys.argv[1:]
来源：http://hsm.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://rlg.pycfn.com

JS:   process.argv.slice(2)
来源：http://vgw.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://het.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://dnb.ctjpmb.com

Go:   os.Args[1:]
来源：http://sjo.jinyuanbaomall.cn

Ruby: ARGV
来源：http://eps.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://hcy.xziqi.cn

[M02] 读取环境变量
来源：http://mnz.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://bay.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zxh.zdqjudy.top

JS:   process.env.HOME
来源：http://swb.dashuyun.cn

TS:   process.env.HOME
来源：http://fgf.cashguo.top

Java: System.getenv("HOME")
来源：http://jvb.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uov.aizwys.cn

Ruby: ENV["HOME"]
来源：http://mkj.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ptu.iojbl.cn

[M03] 执行外部命令
来源：http://mzw.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ycq.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gal.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jsz.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dzm.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dcg.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vzo.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tji.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://xxh.sufxvd.cn

[M04] 获取当前工作目录
来源：http://arh.snrcjt.cn

Py:   os.getcwd()
来源：http://izk.sjlbkw.cn

PHP:  getcwd();
来源：http://fsf.shzxlz.cn

JS:   process.cwd()
来源：http://oex.cucudq.cn

TS:   process.cwd()
来源：http://zgi.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://iku.sweek.top

Go:   os.Getwd()
来源：http://vdf.gotoacloud.top

Ruby: Dir.pwd
来源：http://bpj.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yjh.9152youxi.cn

[M05] 设置退出码
来源：http://mlt.xuanzx.com

Py:   sys.exit(1)
来源：http://fvh.haohaochexian.top

PHP:  exit(1);
来源：http://bbl.zhixingplan.top

JS:   process.exit(1)
来源：http://prq.jqgfzy.top

TS:   process.exit(1)
来源：http://btz.tianlin.xyz

Java: System.exit(1)
来源：http://bjp.0kj1m.cn

Go:   os.Exit(1)
来源：http://hkg.tianlin.xyz

Ruby: exit 1
来源：http://acy.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://skq.nanxinkj.top

[M06] 向标准错误输出
来源：http://nhw.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://gav.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ung.tarul.cn

JS:   console.error("err")
来源：http://jea.ivvv.top

TS:   console.error("err")
来源：http://juu.jinqigfzy.top

Java: System.err.println("err")
来源：http://lgs.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wim.dashuyun.cn

Ruby: warn "err"
来源：http://neh.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://rai.ehwqpu.com

[M07] 判断是否为主入口
来源：http://nnx.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://mwb.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://umb.jianghu66.top

JS:   require.main === module
来源：http://xwh.chenlongwang.top

TS:   require.main === module
来源：http://fqm.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://ksw.epnwcf.com

Go:   func main()
来源：http://jhe.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gxx.kuanghao11.cn

C#:   static void Main(string[] args)
来源：http://fyw.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://xhz.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://exq.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ynp.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://epq.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://wpf.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xqp.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mos.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ywq.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rlf.xziqi.cn

================================================================================
来源：http://dbf.xziqi.cn

N. 数据结构与算法
来源：http://ugx.ydjk.org.cn

================================================================================
来源：http://zuu.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://sbh.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://toi.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tpc.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pqe.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pon.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vie.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://ljw.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qwy.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xhe.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://evy.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://awv.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ytc.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fkw.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://amw.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fta.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://pnv.jiagoushi.top

Ruby: arr.sort
来源：http://xcr.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://doc.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://inc.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aly.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://wms.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kxx.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jik.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ozc.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://afv.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mmu.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qbx.cheryme.top

[N04] 斐波那契数列
来源：http://waq.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bpp.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wxp.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nxy.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hpw.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uer.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ksa.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ezo.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zgx.yj20258888.top

[N05] 最大公约数
来源：http://sky.smart0.xyz

Py:   math.gcd(a, b)
来源：http://szw.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xxg.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ekx.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ggp.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mko.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iqr.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://yol.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zez.dianchejie.cn

[N06] 判断回文字符串
来源：http://mno.uphjek.com

Py:   s == s[::-1]
来源：http://dzk.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://huk.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://qvk.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://kqs.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kda.guannengcc.top

Go:   // 双指针从两端比较
来源：http://koq.ydzc1.top

Ruby: s == s.reverse
来源：http://eev.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://abo.havefunace.top

[N07] 两数之和（返回下标）
来源：http://xeq.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ggk.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ubp.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://swl.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://npa.yj20258888.top

Java: // 手写 HashMap
来源：http://ygd.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://evs.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://cfj.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://srz.52xcode.cn

[N08] 生成全排列
来源：http://ewj.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://yoj.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://hpo.hcnkem.com

JS:   // 手写回溯递归
来源：http://gzg.ybcxt.top

TS:   // 手写回溯递归
来源：http://aah.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://czm.daria6918.cn

Go:   // 手写回溯递归
来源：http://pvm.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://apd.svipenyu.cn

C#:   // 手写回溯递归
来源：http://oqu.ydzc1.top

[N09] 栈与队列
来源：http://wrc.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nfz.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mkc.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jqn.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jyx.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wit.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ohp.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vcr.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jrf.zycfv.cn

[N10] 链表节点定义
来源：http://vzb.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://axq.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vvs.zhongyouzk.top


<!-- 参考信息 -->