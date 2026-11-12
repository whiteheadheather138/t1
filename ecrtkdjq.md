代发 wailian999

TS:   JSON.parse(s)
来源：http://lyq.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zoh.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://fgy.nwbrower.top

Ruby: JSON.parse(s)
来源：http://umu.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ezp.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://ynm.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tem.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://guw.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://unl.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yqe.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ugz.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xib.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://vaj.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://obz.tian-w.cn

[K04] 读取 JSON 文件
来源：http://yhz.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ebx.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jtt.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebs.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hzj.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tzn.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dfk.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mqn.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xaa.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://jtz.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://qxi.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://wbe.sweek.top

JS:   structuredClone(obj)
来源：http://xgh.yj20258.top

TS:   structuredClone(obj)
来源：http://uhq.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qfx.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gag.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aob.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mkm.hnqzz.top

[K06] 解析 URL 查询串
来源：http://lnx.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mbo.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://usm.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyq.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://thr.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://agc.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lbf.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rgx.yueranfly.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ywf.mhx1999.top

[K07] 进制转换
来源：http://dzq.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ceb.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tpq.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://beb.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://afn.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ypn.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vay.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bjm.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sxb.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://feu.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://qwi.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mio.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://wcy.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://pzd.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jpw.gogol.net.cn

Go:   encoding/gob
来源：http://mak.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://wfr.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vnq.0kj1m.cn

================================================================================
来源：http://ivl.yongpay.top

L. 网络请求
来源：http://sfc.yangfankeji.com

================================================================================
来源：http://drs.guowangkeji.top

[L01] 发送 GET 请求
来源：http://iyn.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://riq.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bxd.316326.xyz

JS:   await fetch(url)
来源：http://gva.wangshuangyany.cn

TS:   await fetch(url)
来源：http://uhp.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://una.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://pdb.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oow.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cfr.yueranfly.top

[L02] 发送 POST JSON
来源：http://mgg.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://ldm.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cdx.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hps.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yzg.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rmy.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gcd.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cup.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mjb.tanke756.top

[L03] 设置自定义请求头
来源：http://lgr.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jed.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://thu.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pls.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rip.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ved.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rvv.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tur.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gew.yuanzhike.top

[L04] 设置超时
来源：http://muy.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://lrk.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jzz.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nss.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qhn.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mve.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iji.xinyue.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pbi.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vld.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://qjz.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tcu.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xqf.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yqq.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bml.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://svz.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ubx.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bsr.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hjo.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://uox.nanxuanxn.top

Py:   resp.json()
来源：http://odr.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://jda.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://kaw.hysaishi.cn

TS:   await resp.json()
来源：http://wwt.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bjj.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ojp.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://tvs.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uch.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://pnp.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gyv.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://djs.yj20258.top

JS:   resp.ok;  resp.status
来源：http://ekr.yj20258.top

TS:   resp.ok;  resp.status
来源：http://fdq.haohaochexian.top

Java: resp.statusCode()
来源：http://rvk.bjfxy.top

Go:   resp.StatusCode
来源：http://csj.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://qlg.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://cif.yfazqb.com

[L08] 并发请求多个地址
来源：http://acd.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oml.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://ove.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tjs.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgi.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tpu.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qhi.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fbs.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgu.bbcook.cn

================================================================================
来源：http://pem.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://gqj.xuetiantiany.cn

================================================================================
来源：http://nfv.sufxvd.cn

[M01] 读取命令行参数
来源：http://wbn.xuanzx.com

Py:   sys.argv[1:]
来源：http://zdx.tarul.cn

PHP:  $argv;  $argc;
来源：http://irx.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://ttk.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://lby.tanke756.top

Java: args 数组（main 方法参数）
来源：http://fha.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://pjx.shuidangran.top

Ruby: ARGV
来源：http://aeq.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://wsf.svipenyu.cn

[M02] 读取环境变量
来源：http://brp.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://vei.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dtx.cheryme.top

JS:   process.env.HOME
来源：http://bkh.sjlbkw.cn

TS:   process.env.HOME
来源：http://wri.ehwqpu.com

Java: System.getenv("HOME")
来源：http://umh.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ncs.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://zyq.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://olw.9152youxi.cn

[M03] 执行外部命令
来源：http://gfc.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kat.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qcj.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hgk.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dng.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hhv.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hou.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://rzx.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://qge.yj202588.top

[M04] 获取当前工作目录
来源：http://qpb.sysykeji.top

Py:   os.getcwd()
来源：http://one.hnqzz.top

PHP:  getcwd();
来源：http://sxi.zhixingplan.top

JS:   process.cwd()
来源：http://kfp.jlsjyb.cn

TS:   process.cwd()
来源：http://cih.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://uwt.bbcook.cn

Go:   os.Getwd()
来源：http://fbt.yanxiufei.cn

Ruby: Dir.pwd
来源：http://rmq.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://igl.shuidangran.top

[M05] 设置退出码
来源：http://unk.ppjwa.cn

Py:   sys.exit(1)
来源：http://ivc.yfazqb.com

PHP:  exit(1);
来源：http://dji.daria6918.cn

JS:   process.exit(1)
来源：http://yhv.jqgfzy.top

TS:   process.exit(1)
来源：http://mvr.svipenyu.cn

Java: System.exit(1)
来源：http://ttz.dashuyun.cn

Go:   os.Exit(1)
来源：http://axr.nwbrower.top

Ruby: exit 1
来源：http://wfr.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ntu.iojbl.cn

[M06] 向标准错误输出
来源：http://dym.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://pfh.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://scp.fehbvm.com

JS:   console.error("err")
来源：http://pgn.hnxiangtu.top

TS:   console.error("err")
来源：http://ypb.dashuyun.cn

Java: System.err.println("err")
来源：http://yqu.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kgr.gaohongyu789.top

Ruby: warn "err"
来源：http://kwr.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://nur.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://stg.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://raq.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eye.zhoulong.xyz

JS:   require.main === module
来源：http://bqd.chenjidiqi.icu

TS:   require.main === module
来源：http://zfh.sufxvd.cn

Java: public static void main(String[] args)
来源：http://pzc.52xcode.cn

Go:   func main()
来源：http://yve.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sep.xziqi.cn

C#:   static void Main(string[] args)
来源：http://ibg.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://liw.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://rdm.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://hxz.ybcxt.top

JS:   process.platform;  process.version
来源：http://sxe.52xcode.cn

TS:   process.platform;  process.version
来源：http://zic.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mwj.52xcode.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kbf.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ceh.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://tys.kuanghao11.cn

================================================================================
来源：http://uka.yvedp.cn

N. 数据结构与算法
来源：http://gyd.xingfuxueyuan.xyz

================================================================================
来源：http://xcc.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://cpe.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://ibw.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zzm.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mig.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hlq.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://ztj.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://xgo.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ezy.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://ugx.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://cft.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://cqn.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xot.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mhc.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mre.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vhi.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://vbi.andypj.xyz

Ruby: arr.sort
来源：http://gof.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://usu.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://bki.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://whd.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://jsj.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lbd.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xjx.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rsm.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jpq.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nif.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cbw.ppjwa.cn

[N04] 斐波那契数列
来源：http://dop.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gju.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jwt.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mnh.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pra.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://abj.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qdq.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nyf.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zaw.shangyingyoupin.top

[N05] 最大公约数
来源：http://qkq.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://fsg.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zoy.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rzw.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jvv.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://owv.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zce.vehdjk.com

Ruby: a.gcd(b)
来源：http://wne.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eyu.xinyue.icu

[N06] 判断回文字符串
来源：http://psa.quarkkingdee.top

Py:   s == s[::-1]
来源：http://xuc.316326.xyz

PHP:  $s === strrev($s);
来源：http://lkf.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://bop.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://qbt.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gdf.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://vcs.iojbl.cn

Ruby: s == s.reverse
来源：http://ymr.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ohj.yj202588.top

[N07] 两数之和（返回下标）
来源：http://izy.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ppw.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kcz.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kuk.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://exh.zhixingplan.top

Java: // 手写 HashMap
来源：http://efs.tian-w.cn

Go:   // 手写 map[int]int
来源：http://mwf.jyoumei.cn

Ruby: // 手写 Hash
来源：http://usm.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ofr.jqgufenzy.top

[N08] 生成全排列
来源：http://gnk.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://gfq.vehdjk.com

PHP:  // 手写递归交换
来源：http://svh.52xcode.cn

JS:   // 手写回溯递归
来源：http://vzb.yj202588.top

TS:   // 手写回溯递归
来源：http://bcm.zhijiandao.cn

Java: // 手写回溯递归
来源：http://cig.guannengcc.top

Go:   // 手写回溯递归
来源：http://ekl.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://hzx.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://hek.hnxiangtu.top

[N09] 栈与队列
来源：http://oos.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://swl.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tyo.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qad.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://enw.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yuy.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kte.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zjr.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdw.bjfxy.top

[N10] 链表节点定义
来源：http://xng.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dux.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rhs.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wwr.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zln.meibo888.top

Java: class Node { int v; Node next; }
来源：http://fht.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://msu.xuanzx.com


<!-- 参考信息 -->