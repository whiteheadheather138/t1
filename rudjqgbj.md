代发 wailian999

[K02] JSON 字符串转对象
来源：http://ved.yuxming.cn

Py:   json.loads(s)
来源：http://jis.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kdf.fzhhl.top

JS:   JSON.parse(s)
来源：http://mze.sweek.top

TS:   JSON.parse(s)
来源：http://goh.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cvg.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://qrd.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://mxj.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cho.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://nuk.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qnd.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ynf.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gle.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pav.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://prz.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oje.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://elp.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://krm.andypj.xyz

[K04] 读取 JSON 文件
来源：http://pfz.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wes.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oys.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jxh.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hvn.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wqb.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zws.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://itm.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hbf.tanke756.top

[K05] 深拷贝对象
来源：http://cxf.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://xyg.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://rhe.hammf.cn

JS:   structuredClone(obj)
来源：http://fvi.wangdashe.top

TS:   structuredClone(obj)
来源：http://rrx.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://jmy.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://siq.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zlt.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uzt.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://uuz.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rhu.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jbu.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sot.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://phx.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uzn.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bzi.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zgv.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rrc.nanxuanxn.top

[K07] 进制转换
来源：http://nox.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://krk.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sjh.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xhx.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://afs.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sac.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fxs.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yrn.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dmh.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://gcp.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://haq.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dog.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://whg.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://jdq.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lla.birdmap.top

Go:   encoding/gob
来源：http://sar.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://tlt.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iyq.yvedp.cn

================================================================================
来源：http://agv.xuetiantiany.cn

L. 网络请求
来源：http://fxc.hnqzz.top

================================================================================
来源：http://osw.bbcook.cn

[L01] 发送 GET 请求
来源：http://mfj.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kff.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yqs.c1oappe.top

JS:   await fetch(url)
来源：http://xxw.cdnleiting.top

TS:   await fetch(url)
来源：http://ihe.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vvp.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://glw.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ihx.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wmt.yj20258.top

[L02] 发送 POST JSON
来源：http://xjw.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://mit.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ggg.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mde.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jbw.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vgb.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cdf.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hhw.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hju.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://qym.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tro.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pgb.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbl.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rmr.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bam.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kfx.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://neq.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://msw.xuanzx.com

[L04] 设置超时
来源：http://qen.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://nom.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tcp.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://egi.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wlw.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eft.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oli.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qxm.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fmg.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://the.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xii.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mhy.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://naa.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nic.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dhb.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gho.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mzc.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dgb.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://wyg.sysykeji.top

Py:   resp.json()
来源：http://fgg.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://zoz.xuetiantiany.cn

JS:   await resp.json()
来源：http://ynw.iojbl.cn

TS:   await resp.json()
来源：http://ezw.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jkh.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ich.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://sgj.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uzs.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://vcr.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wfp.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kzw.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://cvu.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://lvf.zycfv.cn

Java: resp.statusCode()
来源：http://hah.jqgfzy.top

Go:   resp.StatusCode
来源：http://png.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://uzl.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://uxp.52xcode.cn

[L08] 并发请求多个地址
来源：http://esl.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sru.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://zgi.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xse.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fbg.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gdc.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yjk.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uxc.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eky.shuidangran.top

================================================================================
来源：http://jmg.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://ezp.jqgufenzy.top

================================================================================
来源：http://dcr.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://fpe.cdnleiting.top

Py:   sys.argv[1:]
来源：http://zys.epnwcf.com

PHP:  $argv;  $argc;
来源：http://von.cheryme.top

JS:   process.argv.slice(2)
来源：http://rjw.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://rov.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://apx.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://xxb.gzhubu.top

Ruby: ARGV
来源：http://qqx.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://bxi.316326.xyz

[M02] 读取环境变量
来源：http://nta.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://ebq.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://huz.yueranfly.top

JS:   process.env.HOME
来源：http://xfs.yueranfly.top

TS:   process.env.HOME
来源：http://yuj.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://mtk.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bqv.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://jby.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sxk.yuanzhike.top

[M03] 执行外部命令
来源：http://glh.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hvr.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nwz.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jrk.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ymm.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hdb.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bxk.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://gpy.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://nfg.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://jxe.andypj.xyz

Py:   os.getcwd()
来源：http://rxx.9152youxi.cn

PHP:  getcwd();
来源：http://gko.c1oappe.top

JS:   process.cwd()
来源：http://gzx.dianchejie.cn

TS:   process.cwd()
来源：http://jdo.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://jwk.aizwys.cn

Go:   os.Getwd()
来源：http://jwv.ppjwa.cn

Ruby: Dir.pwd
来源：http://nzy.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://sdj.jiagoushi.top

[M05] 设置退出码
来源：http://exp.hesvh.cn

Py:   sys.exit(1)
来源：http://rks.hnqzz.top

PHP:  exit(1);
来源：http://qyc.daxiang520.top

JS:   process.exit(1)
来源：http://hoa.fengsongda.top

TS:   process.exit(1)
来源：http://qtn.yuanzhike.top

Java: System.exit(1)
来源：http://bec.0kj1m.cn

Go:   os.Exit(1)
来源：http://nuw.yj202588.top

Ruby: exit 1
来源：http://lur.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nio.zhijiandao.cn

[M06] 向标准错误输出
来源：http://jid.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://rbe.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://glg.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://bxk.hnqzz.top

TS:   console.error("err")
来源：http://how.svipenyu.cn

Java: System.err.println("err")
来源：http://keq.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pyz.chenlongwang.top

Ruby: warn "err"
来源：http://xax.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://wxt.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://ewa.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://iim.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rzu.yvedp.cn

JS:   require.main === module
来源：http://hrr.yongpay.top

TS:   require.main === module
来源：http://vfx.hysaishi.cn

Java: public static void main(String[] args)
来源：http://qfp.ppjwa.cn

Go:   func main()
来源：http://kjc.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xsd.pycfn.com

C#:   static void Main(string[] args)
来源：http://kjo.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://vus.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://rcz.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://gvt.xziqi.cn

JS:   process.platform;  process.version
来源：http://hwl.yj20258.top

TS:   process.platform;  process.version
来源：http://xth.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jkn.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kma.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fmg.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xhe.cheryme.top

================================================================================
来源：http://mvj.haohaochexian.top

N. 数据结构与算法
来源：http://lsv.gogol.net.cn

================================================================================
来源：http://vbx.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://woa.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://yls.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sbx.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://svt.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hru.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://nnk.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://cds.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://knq.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nhq.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://nxd.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://yno.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ijj.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eiw.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sha.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dne.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://duq.hnqzz.top

Ruby: arr.sort
来源：http://odh.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://zpg.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://ecp.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zie.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://sre.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lis.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gvc.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ejp.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ltg.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ofq.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://mtu.daria6918.cn

[N04] 斐波那契数列
来源：http://ela.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bsd.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tcw.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tsc.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dfw.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sdf.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ezd.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rus.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nkj.smart0.xyz

[N05] 最大公约数
来源：http://tqa.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://zqh.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jca.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bfl.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mnl.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iby.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ldf.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://vfe.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://keq.yj20258888.top

[N06] 判断回文字符串
来源：http://oup.tarul.cn

Py:   s == s[::-1]
来源：http://tsz.tanke756.top

PHP:  $s === strrev($s);
来源：http://mut.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://aub.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://wwj.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dxo.zycfv.cn

Go:   // 双指针从两端比较
来源：http://uwz.zhijiandao.cn

Ruby: s == s.reverse
来源：http://mig.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bnw.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://uej.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://upk.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://egj.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nsx.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://zee.yueranfly.top

Java: // 手写 HashMap
来源：http://fky.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://kve.gzhubu.top

Ruby: // 手写 Hash
来源：http://smi.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://ina.redwolf501.top

[N08] 生成全排列
来源：http://xis.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://fmz.52xcode.cn

PHP:  // 手写递归交换
来源：http://yxg.meibo888.top

JS:   // 手写回溯递归
来源：http://dde.andypj.xyz

TS:   // 手写回溯递归
来源：http://dja.chenlongwang.top

Java: // 手写回溯递归
来源：http://bmv.fktsv.cn

Go:   // 手写回溯递归
来源：http://xkd.uphjek.com

Ruby: arr.permutation.to_a
来源：http://wvs.mhx1999.top

C#:   // 手写回溯递归
来源：http://uxj.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://duc.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hap.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ziu.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vuw.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sgk.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fcg.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kxs.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://arw.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cff.jlsjyb.cn

[N10] 链表节点定义
来源：http://xym.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yhu.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ywj.zhijiandao.cn


<!-- 参考信息 -->