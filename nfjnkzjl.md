代发 wailian999

TS:   JSON.parse(s)
来源：http://dzk.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qmd.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://dqa.tarul.cn

Ruby: JSON.parse(s)
来源：http://ahl.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uqy.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://ngr.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hjy.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ikk.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qim.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ibb.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gan.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gip.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qnr.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gse.fehbvm.com

[K04] 读取 JSON 文件
来源：http://scm.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tyf.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://igu.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://esa.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://udd.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bxs.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qms.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://buo.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qxx.sweek.top

[K05] 深拷贝对象
来源：http://ngj.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://krz.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://wyh.wangdashe.top

JS:   structuredClone(obj)
来源：http://gxl.chenlongwang.top

TS:   structuredClone(obj)
来源：http://esf.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sum.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ziv.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qoa.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nst.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://zkd.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vzp.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://chz.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzg.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wgd.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wmg.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hru.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dio.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rps.xziqi.cn

[K07] 进制转换
来源：http://vqb.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gwf.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kti.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ypx.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ett.kuanghao11.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ias.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gsk.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ucx.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://spi.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://wti.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://ekq.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://hea.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://atx.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ebz.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wad.sysykeji.top

Go:   encoding/gob
来源：http://luw.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://bis.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sgy.zdqjudy.top

================================================================================
来源：http://yyu.quarkkingdee.top

L. 网络请求
来源：http://cga.fktsv.cn

================================================================================
来源：http://nna.chenlongwang.top

[L01] 发送 GET 请求
来源：http://srn.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://neb.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hor.zdbjq.cn

JS:   await fetch(url)
来源：http://kes.snrcjt.cn

TS:   await fetch(url)
来源：http://eub.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ghl.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://myn.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jkx.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rpe.havefunace.top

[L02] 发送 POST JSON
来源：http://tbn.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://yif.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xxp.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bgr.cdnleiting.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bgn.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tia.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://buf.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fxz.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xuv.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://ctk.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hyy.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sxz.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rsv.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ref.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ayc.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dpa.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sks.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dbe.zhengqikj.top

[L04] 设置超时
来源：http://gse.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://lyx.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dus.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dqo.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zag.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yuv.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://loz.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yol.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://igy.yongpay.top

[L05] 上传文件（multipart）
来源：http://apd.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wuh.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jrh.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jdv.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kcf.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nxy.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wvy.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wfz.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iat.yongpay.top

[L06] 解析响应为 JSON
来源：http://reg.kuanghao11.cn

Py:   resp.json()
来源：http://vcy.cucudq.cn

PHP:  json_decode($body, true);
来源：http://abe.xinyue.icu

JS:   await resp.json()
来源：http://utf.yuxming.cn

TS:   await resp.json()
来源：http://lvt.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://spk.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jbj.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://izk.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://khq.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://ddq.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kto.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jgh.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://afn.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://vvk.yj20258888.top

Java: resp.statusCode()
来源：http://xuo.hesvh.cn

Go:   resp.StatusCode
来源：http://ljf.andypj.xyz

Ruby: resp.code.to_i
来源：http://wqw.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://hql.ehwqpu.com

[L08] 并发请求多个地址
来源：http://jwp.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yvc.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://mkw.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qyg.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xvm.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lzz.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ptt.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oxs.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vyr.cqqwz.cn

================================================================================
来源：http://wca.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://mqg.daxiang520.top

================================================================================
来源：http://bhz.jlsjyb.cn

[M01] 读取命令行参数
来源：http://sln.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://jsv.yj20258888.top

PHP:  $argv;  $argc;
来源：http://kev.jianghu66.top

JS:   process.argv.slice(2)
来源：http://dwb.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://lep.tarul.cn

Java: args 数组（main 方法参数）
来源：http://qvo.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://xmd.jqgfzy.top

Ruby: ARGV
来源：http://bom.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://nkz.hfpthk.cn

[M02] 读取环境变量
来源：http://tlw.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://hqo.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mhe.daria6918.cn

JS:   process.env.HOME
来源：http://fjd.uphjek.com

TS:   process.env.HOME
来源：http://isf.52xcode.cn

Java: System.getenv("HOME")
来源：http://pma.nwbrower.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nkt.xylfe.cn

Ruby: ENV["HOME"]
来源：http://iat.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://esu.yongpay.top

[M03] 执行外部命令
来源：http://lng.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://not.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rpr.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sxo.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nww.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://knd.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lio.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fqh.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://ptx.yueranfly.top

[M04] 获取当前工作目录
来源：http://pcm.chenzaomai.com

Py:   os.getcwd()
来源：http://clo.shzxlz.cn

PHP:  getcwd();
来源：http://win.yueranfly.top

JS:   process.cwd()
来源：http://dkf.ivvv.top

TS:   process.cwd()
来源：http://gsp.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://vlc.hammf.cn

Go:   os.Getwd()
来源：http://fsn.cqqwz.cn

Ruby: Dir.pwd
来源：http://hyp.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://qye.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://pmn.yueranfly.top

Py:   sys.exit(1)
来源：http://qiw.dashuyun.cn

PHP:  exit(1);
来源：http://hfn.sufxvd.cn

JS:   process.exit(1)
来源：http://ana.yfazqb.com

TS:   process.exit(1)
来源：http://wpr.xuetiantiany.cn

Java: System.exit(1)
来源：http://rtf.xinyue.icu

Go:   os.Exit(1)
来源：http://cwv.gaohongyu789.top

Ruby: exit 1
来源：http://zqj.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rvl.tarul.cn

[M06] 向标准错误输出
来源：http://wvr.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://tvt.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bey.dianchejie.cn

JS:   console.error("err")
来源：http://wuk.guannengcc.top

TS:   console.error("err")
来源：http://lwf.yfazqb.com

Java: System.err.println("err")
来源：http://ccu.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yrw.zycfv.cn

Ruby: warn "err"
来源：http://tot.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://htl.redwolf501.top

[M07] 判断是否为主入口
来源：http://eav.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://pal.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eqt.chenlongwang.top

JS:   require.main === module
来源：http://lwl.tanke756.top

TS:   require.main === module
来源：http://kbo.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://prp.shanyushiyangkeji.top

Go:   func main()
来源：http://ewg.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vno.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://nwu.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://ior.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://ysh.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://dgn.hfpthk.cn

JS:   process.platform;  process.version
来源：http://zgx.gotoacloud.top

TS:   process.platform;  process.version
来源：http://grq.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xnd.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pen.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://are.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://goa.bjfxy.top

================================================================================
来源：http://dwm.hcnkem.com

N. 数据结构与算法
来源：http://knx.sufxvd.cn

================================================================================
来源：http://cpy.aizwys.cn

[N01] 二分查找（有序数组）
来源：http://ysn.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://epz.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ryl.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zej.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cbo.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kfo.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://lzl.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ndc.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://gmf.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://jlc.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://icl.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uzt.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://era.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fjc.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uri.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://gsh.tarul.cn

Ruby: arr.sort
来源：http://dzv.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://hpq.sysykeji.top

[N03] 快速排序（分治示例）
来源：http://sqp.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rmg.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://pux.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aqk.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://njv.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hxd.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://utx.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://icf.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://orw.xinyue.icu

[N04] 斐波那契数列
来源：http://hzw.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hyt.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qbf.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dnk.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fvd.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wcx.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lwd.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wmt.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zkz.iojbl.cn

[N05] 最大公约数
来源：http://lqr.cheryme.top

Py:   math.gcd(a, b)
来源：http://wxq.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pdu.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mul.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xez.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lsc.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vgz.yuxming.cn

Ruby: a.gcd(b)
来源：http://yzd.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pmi.gotoacloud.top

[N06] 判断回文字符串
来源：http://ezf.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://wzn.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://pah.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://ewi.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://jgf.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://syw.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://jqx.quarkkingdee.top

Ruby: s == s.reverse
来源：http://irf.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bfd.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://afc.nanxuanxn.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ajr.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cuz.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vwb.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://toi.cdnleiting.top

Java: // 手写 HashMap
来源：http://qfk.yj20258888.top

Go:   // 手写 map[int]int
来源：http://qzu.redwolf501.top

Ruby: // 手写 Hash
来源：http://awo.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://gsm.feifeiyinyue.top

[N08] 生成全排列
来源：http://chq.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://ilh.ydzc1.top

PHP:  // 手写递归交换
来源：http://rhd.daria6918.cn

JS:   // 手写回溯递归
来源：http://wug.gotoacloud.top

TS:   // 手写回溯递归
来源：http://ngr.yuxming.cn

Java: // 手写回溯递归
来源：http://rdc.yfazqb.com

Go:   // 手写回溯递归
来源：http://dgy.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://rmu.zhengqikj.top

C#:   // 手写回溯递归
来源：http://umz.yonumen.top

[N09] 栈与队列
来源：http://tdz.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lyz.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hxq.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hlo.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qsn.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tmn.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vva.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://usg.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fsl.hfpthk.cn

[N10] 链表节点定义
来源：http://mbm.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gdq.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jct.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gjc.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jhd.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://rqx.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://wiy.zdbjq.cn


<!-- 参考信息 -->