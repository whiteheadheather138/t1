代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ohe.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://ftp.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rfx.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iaf.svipenyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://znq.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hhl.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aic.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zyk.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://ven.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oho.cashguo.top

[K04] 读取 JSON 文件
来源：http://axw.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bot.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mmo.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vvc.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ibd.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ymu.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kha.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dxt.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cca.yongpay.top

[K05] 深拷贝对象
来源：http://rog.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://udw.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://wdu.birdmap.top

JS:   structuredClone(obj)
来源：http://grj.pycfn.com

TS:   structuredClone(obj)
来源：http://hdm.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mxg.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yki.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zql.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qsg.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://vdm.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pns.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aya.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wkj.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvu.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hdw.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fim.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bxu.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cpw.ybcxt.top

[K07] 进制转换
来源：http://jno.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hqi.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ukw.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pgs.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kaf.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xfy.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mti.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ups.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xxk.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://ajh.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://kmj.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://eif.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://blj.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://ije.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fcg.zycfv.cn

Go:   encoding/gob
来源：http://ikk.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://tju.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xjd.andypj.xyz

================================================================================
来源：http://qyj.tianlin.xyz

L. 网络请求
来源：http://tgy.9152youxi.cn

================================================================================
来源：http://zph.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://sdr.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bho.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://noj.daria6918.cn

JS:   await fetch(url)
来源：http://fvv.shangyingyoupin.top

TS:   await fetch(url)
来源：http://coy.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wqv.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://yuq.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tbo.hammf.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ucy.guannengcc.top

[L02] 发送 POST JSON
来源：http://cpa.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://dmp.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://prb.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wdj.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uwj.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wcx.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nwo.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gfy.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aki.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://knr.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rie.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mrb.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kgu.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agq.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eks.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vzd.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wqj.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://teh.fktsv.cn

[L04] 设置超时
来源：http://rvv.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://keg.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dnk.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tnr.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lze.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vag.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bts.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bxh.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://huq.haohaochexian.top

[L05] 上传文件（multipart）
来源：http://gcd.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ofq.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uek.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://byn.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mux.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nnz.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baa.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ymn.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://unu.tanke756.top

[L06] 解析响应为 JSON
来源：http://ogk.vqdsnc.cn

Py:   resp.json()
来源：http://zfu.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://fym.316326.xyz

JS:   await resp.json()
来源：http://atu.ctjpmb.com

TS:   await resp.json()
来源：http://aml.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://izd.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zpu.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://jzy.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uyp.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://ref.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://psl.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pmb.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://zkq.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://jxs.hnqzz.top

Java: resp.statusCode()
来源：http://ndb.gaohongyu789.top

Go:   resp.StatusCode
来源：http://bmw.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://abb.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://qta.yj20258888.top

[L08] 并发请求多个地址
来源：http://djt.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gpv.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://tfw.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://men.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bhb.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dsn.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sww.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ewy.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aam.ivvv.top

================================================================================
来源：http://moi.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://sst.gaohongyu789.top

================================================================================
来源：http://ogt.yfazqb.com

[M01] 读取命令行参数
来源：http://hvj.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://ene.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://jvb.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://iik.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://pik.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://dst.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://vqd.sweek.top

Ruby: ARGV
来源：http://nbv.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://spb.fehbvm.com

[M02] 读取环境变量
来源：http://xpc.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://aid.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ivc.snrcjt.cn

JS:   process.env.HOME
来源：http://txj.guannengcc.top

TS:   process.env.HOME
来源：http://vfr.ydzc1.top

Java: System.getenv("HOME")
来源：http://nxr.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mbq.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://zmw.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://att.shuidangran.top

[M03] 执行外部命令
来源：http://lua.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hmo.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rve.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nbu.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dmb.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ecw.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://zyh.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://fmb.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://nka.jiagoushi.top

[M04] 获取当前工作目录
来源：http://nff.fzhhl.top

Py:   os.getcwd()
来源：http://djk.jinqigfzy.top

PHP:  getcwd();
来源：http://gdg.pengpengdd.cyou

JS:   process.cwd()
来源：http://ubx.shzxlz.cn

TS:   process.cwd()
来源：http://mnw.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://nou.tian-w.cn

Go:   os.Getwd()
来源：http://bir.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://uft.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ujc.chenlongwang.top

[M05] 设置退出码
来源：http://odc.fzhhl.top

Py:   sys.exit(1)
来源：http://auv.ydjk.org.cn

PHP:  exit(1);
来源：http://koz.zycfv.cn

JS:   process.exit(1)
来源：http://ndm.fktsv.cn

TS:   process.exit(1)
来源：http://spz.sufxvd.cn

Java: System.exit(1)
来源：http://hki.yonumen.top

Go:   os.Exit(1)
来源：http://vzu.jqgufenzy.top

Ruby: exit 1
来源：http://bix.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pee.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://bkw.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://sfs.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rtf.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://pnu.hongshengwenyu.top

TS:   console.error("err")
来源：http://xte.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://ssv.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://piu.jianghu66.top

Ruby: warn "err"
来源：http://yax.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://nju.ybcxt.top

[M07] 判断是否为主入口
来源：http://evr.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://kbq.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zhs.andypj.xyz

JS:   require.main === module
来源：http://twg.ywan-chungtsiang.top

TS:   require.main === module
来源：http://bzb.yonumen.top

Java: public static void main(String[] args)
来源：http://smy.fehbvm.com

Go:   func main()
来源：http://zaf.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ccx.fktsv.cn

C#:   static void Main(string[] args)
来源：http://hko.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://rsz.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://xtc.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://dur.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://zrm.pycfn.com

TS:   process.platform;  process.version
来源：http://ori.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ehz.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uxo.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lbf.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://slw.hnxiangtu.top

================================================================================
来源：http://tea.shzxlz.cn

N. 数据结构与算法
来源：http://vqs.nanxuanxn.top

================================================================================
来源：http://rso.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://xip.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://snd.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vtf.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ujn.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vdl.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://uwu.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://oxk.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fdt.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://xol.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://sqz.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://emh.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ogc.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wfg.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nfs.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hzd.hesvh.cn

Go:   slices.Sort(arr)
来源：http://yvm.zhixingplan.top

Ruby: arr.sort
来源：http://qtl.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pan.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://zje.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rzw.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://ytt.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qiw.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qep.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mmm.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ves.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rmv.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://bgh.hammf.cn

[N04] 斐波那契数列
来源：http://qld.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lsg.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yiy.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ihv.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sfg.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://suq.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cje.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wjj.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jvq.xuetiantiany.cn

[N05] 最大公约数
来源：http://nhh.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://hgw.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hcg.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iol.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vds.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tza.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zxz.cdnleiting.top

Ruby: a.gcd(b)
来源：http://byc.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://udt.fzhhl.top

[N06] 判断回文字符串
来源：http://kmq.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://ldh.xinyue.icu

PHP:  $s === strrev($s);
来源：http://vbh.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://swv.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://rns.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvc.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://axj.hysaishi.cn

Ruby: s == s.reverse
来源：http://lsg.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wge.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://uie.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://imk.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ant.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://hoq.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://zxn.dashuyun.cn

Java: // 手写 HashMap
来源：http://guo.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://zpm.haohaochexian.top

Ruby: // 手写 Hash
来源：http://kjt.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cmb.uphjek.com

[N08] 生成全排列
来源：http://tzq.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://pop.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://roy.hywenlv.cn

JS:   // 手写回溯递归
来源：http://zhi.gotoacloud.top

TS:   // 手写回溯递归
来源：http://zer.yj202588.top

Java: // 手写回溯递归
来源：http://msm.hfpthk.cn

Go:   // 手写回溯递归
来源：http://gpe.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://rds.mhx1999.top

C#:   // 手写回溯递归
来源：http://cwc.quarkkingdee.top

[N09] 栈与队列
来源：http://gqs.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kxn.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cjb.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://peu.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kye.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zqk.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zqf.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uaa.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lzy.9152youxi.cn

[N10] 链表节点定义
来源：http://kxh.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bmc.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bls.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sqy.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nhu.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://qgh.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://twm.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jlb.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://osr.sysykeji.top

[N11] 二叉树中序遍历
来源：http://qle.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iiy.jianghu66.top


<!-- 参考信息 -->