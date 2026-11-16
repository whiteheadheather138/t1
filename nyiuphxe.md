代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hya.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://ptx.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bpf.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aap.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://puk.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oqj.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jzz.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gpy.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://fjj.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xnf.yj20258888.top

[K04] 读取 JSON 文件
来源：http://cgx.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hiv.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xjl.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mtp.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rce.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wvo.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hpv.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://myh.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://okv.yangfankeji.com

[K05] 深拷贝对象
来源：http://hhs.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://crg.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://qte.jyoumei.cn

JS:   structuredClone(obj)
来源：http://swt.yuanzhike.top

TS:   structuredClone(obj)
来源：http://ogx.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://exv.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xho.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gvi.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tai.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://lun.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://muh.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wso.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gmv.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrs.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kqp.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kqz.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rbc.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ami.zhoulong.xyz

[K07] 进制转换
来源：http://uuh.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fdo.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dhm.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gxt.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qvb.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wau.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xwu.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bzm.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://enp.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://rcn.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://zoi.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ssv.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://oak.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://yxm.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lyh.gzhubu.top

Go:   encoding/gob
来源：http://nhn.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://wtj.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ebu.xuanzx.com

================================================================================
来源：http://nuf.cashguo.top

L. 网络请求
来源：http://slr.ehwqpu.com

================================================================================
来源：http://mnq.cdnleiting.top

[L01] 发送 GET 请求
来源：http://pao.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jte.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://plc.pycfn.com

JS:   await fetch(url)
来源：http://imo.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://ppd.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mmz.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://yqf.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ogb.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dih.hcnkem.com

[L02] 发送 POST JSON
来源：http://gbz.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://txk.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vjs.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uxe.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vre.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ezo.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xod.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nnk.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lzb.cheryme.top

[L03] 设置自定义请求头
来源：http://lkm.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nwz.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kqk.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zuf.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eci.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eru.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dbl.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://djd.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uax.hammf.cn

[L04] 设置超时
来源：http://iqx.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://ksf.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cji.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tfp.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zuw.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pat.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nid.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xka.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://buq.daxiang520.top

[L05] 上传文件（multipart）
来源：http://vrx.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mje.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://atq.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://azh.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lwe.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mmi.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iru.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tpn.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://viu.hesvh.cn

[L06] 解析响应为 JSON
来源：http://jzg.zhijiandao.cn

Py:   resp.json()
来源：http://bup.yueranfly.top

PHP:  json_decode($body, true);
来源：http://lcq.jinqigfzy.top

JS:   await resp.json()
来源：http://mac.jianghu66.top

TS:   await resp.json()
来源：http://lbb.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ycl.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eqb.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://fhh.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iyl.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://yke.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wkh.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://msi.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://yiv.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://vdr.0kj1m.cn

Java: resp.statusCode()
来源：http://bgz.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://zfm.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://qwe.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://lhc.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://get.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uuj.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://fxz.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vza.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rbd.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ezf.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nzf.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://trf.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xjq.smart0.xyz

================================================================================
来源：http://pqs.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://eli.snrcjt.cn

================================================================================
来源：http://taw.ppjwa.cn

[M01] 读取命令行参数
来源：http://clx.zhengqikj.top

Py:   sys.argv[1:]
来源：http://rtn.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://rxi.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://ryh.yuxming.cn

TS:   process.argv.slice(2)
来源：http://ogo.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://gwk.hnxiangtu.top

Go:   os.Args[1:]
来源：http://unv.svipenyu.cn

Ruby: ARGV
来源：http://iuy.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://dbk.meibo888.top

[M02] 读取环境变量
来源：http://trt.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://ols.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xpk.pycfn.com

JS:   process.env.HOME
来源：http://bkh.svipenyu.cn

TS:   process.env.HOME
来源：http://ocx.tarul.cn

Java: System.getenv("HOME")
来源：http://kwb.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qcl.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://wfy.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mvx.chenzaomai.com

[M03] 执行外部命令
来源：http://nyu.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wsg.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yox.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ira.tanke756.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ick.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://chu.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ysq.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xlx.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://rjm.jiagoushi.top

[M04] 获取当前工作目录
来源：http://gwp.jqgufenzy.top

Py:   os.getcwd()
来源：http://vot.zhiwuduotai.top

PHP:  getcwd();
来源：http://ldn.yonumen.top

JS:   process.cwd()
来源：http://mki.0kj1m.cn

TS:   process.cwd()
来源：http://foi.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://axb.yj20258888.top

Go:   os.Getwd()
来源：http://hyx.yongpay.top

Ruby: Dir.pwd
来源：http://lbj.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://lru.jinqigufen.top

[M05] 设置退出码
来源：http://kxx.hnxiangtu.top

Py:   sys.exit(1)
来源：http://yha.smart0.xyz

PHP:  exit(1);
来源：http://amz.yangfankeji.com

JS:   process.exit(1)
来源：http://onl.yueranfly.top

TS:   process.exit(1)
来源：http://emb.andypj.xyz

Java: System.exit(1)
来源：http://njh.gogol.net.cn

Go:   os.Exit(1)
来源：http://wap.jiagoushi.top

Ruby: exit 1
来源：http://zpz.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxh.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://jan.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://mhn.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://upi.c1oappe.top

JS:   console.error("err")
来源：http://eky.yueranfly.top

TS:   console.error("err")
来源：http://arr.ydjk.org.cn

Java: System.err.println("err")
来源：http://arv.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://arr.fktsv.cn

Ruby: warn "err"
来源：http://okd.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://pni.shzxlz.cn

[M07] 判断是否为主入口
来源：http://mvz.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://qac.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rsn.zhongyouzk.top

JS:   require.main === module
来源：http://lmb.uphjek.com

TS:   require.main === module
来源：http://zda.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://qio.aizwys.cn

Go:   func main()
来源：http://pgh.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qct.fktsv.cn

C#:   static void Main(string[] args)
来源：http://dml.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://anx.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://wcg.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://lgq.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://uqx.bbcook.cn

TS:   process.platform;  process.version
来源：http://org.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kcd.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://moc.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://viu.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://obe.smart0.xyz

================================================================================
来源：http://uef.316326.xyz

N. 数据结构与算法
来源：http://fgs.xylfe.cn

================================================================================
来源：http://vyr.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://nss.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bbd.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://snw.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzb.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jbz.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gnk.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://cfo.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://nkh.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://onr.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://ymg.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://jia.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qmp.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wxr.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bsv.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dij.yonumen.top

Go:   slices.Sort(arr)
来源：http://rjg.hammf.cn

Ruby: arr.sort
来源：http://xqf.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://job.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://mum.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bqq.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://rft.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bfm.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://osu.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nal.haohaochexian.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://has.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://znj.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://kgd.epnwcf.com

[N04] 斐波那契数列
来源：http://hpd.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bwe.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tbh.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iqb.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qjg.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://weu.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://inb.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yiq.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nru.vqdsnc.cn

[N05] 最大公约数
来源：http://gad.xylfe.cn

Py:   math.gcd(a, b)
来源：http://ckb.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fjs.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kzg.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfq.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ytk.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qol.yangfankeji.com

Ruby: a.gcd(b)
来源：http://mgh.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qug.tianlin.xyz

[N06] 判断回文字符串
来源：http://rqy.uphjek.com

Py:   s == s[::-1]
来源：http://hnn.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://bex.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://ynx.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://oit.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rwb.xziqi.cn

Go:   // 双指针从两端比较
来源：http://tye.c1oappe.top

Ruby: s == s.reverse
来源：http://phw.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rup.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://sch.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xxa.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pgn.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wsl.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://oli.yj20258888.top

Java: // 手写 HashMap
来源：http://ide.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://qrb.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://gtg.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://jgd.daxiang520.top

[N08] 生成全排列
来源：http://hgi.hammf.cn

Py:   itertools.permutations(arr)
来源：http://brs.zhengqikj.top

PHP:  // 手写递归交换
来源：http://hce.jiagoushi.top

JS:   // 手写回溯递归
来源：http://yct.yj202588.top

TS:   // 手写回溯递归
来源：http://yph.havefunace.top

Java: // 手写回溯递归
来源：http://rrf.smart0.xyz

Go:   // 手写回溯递归
来源：http://fhn.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://wje.daxiang520.top

C#:   // 手写回溯递归
来源：http://wgd.yuxming.cn

[N09] 栈与队列
来源：http://trg.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://scx.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ujh.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cuf.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ehp.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vvy.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oiu.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://woo.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://onz.ydjk.org.cn

[N10] 链表节点定义
来源：http://inq.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hnk.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cgj.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lug.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zzy.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://qua.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bop.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bzt.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kxf.xziqi.cn

[N11] 二叉树中序遍历
来源：http://jvl.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sid.chenjidiqi.icu


<!-- 参考信息 -->