代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hgy.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://gez.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ryl.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://doa.vehdjk.com

[K02] JSON 字符串转对象
来源：http://cna.redwolf501.top

Py:   json.loads(s)
来源：http://jao.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ohs.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://uti.sxryk.cn

TS:   JSON.parse(s)
来源：http://siy.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://htx.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://qet.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://ral.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jmj.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://fib.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jah.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://prn.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oej.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ply.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iwy.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://upw.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://kua.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jvd.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://yhq.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gwk.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hxq.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nbs.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://chr.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ora.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mep.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lat.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kdw.c1oappe.top

[K05] 深拷贝对象
来源：http://abf.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://zid.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://ety.sxryk.cn

JS:   structuredClone(obj)
来源：http://ltj.chenzaomai.com

TS:   structuredClone(obj)
来源：http://elt.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qhf.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ual.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dwe.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qdq.havefunace.top

[K06] 解析 URL 查询串
来源：http://kcn.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vix.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tur.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xrh.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mqv.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hfp.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eud.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ubt.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jdo.zdbjq.cn

[K07] 进制转换
来源：http://ywj.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vck.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nqp.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uzv.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gak.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ezi.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ccy.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ink.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gyz.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://qho.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://uvm.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pey.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://dsy.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://foi.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zpl.wangshuangyany.cn

Go:   encoding/gob
来源：http://vyx.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://whq.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://otr.zhongyouzk.top

================================================================================
来源：http://gvw.birdmap.top

L. 网络请求
来源：http://dnb.ivvv.top

================================================================================
来源：http://ctr.cashguo.top

[L01] 发送 GET 请求
来源：http://qqc.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ynb.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pvs.hongshengwenyu.top

JS:   await fetch(url)
来源：http://itp.yongpay.top

TS:   await fetch(url)
来源：http://yvh.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gwz.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://tav.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ltg.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gqw.sxryk.cn

[L02] 发送 POST JSON
来源：http://ozl.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://hof.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ham.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qns.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zuw.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zyu.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gur.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aah.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qkj.yanxiufei.cn

[L03] 设置自定义请求头
来源：http://weq.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://biq.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ukx.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbi.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hfh.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uzf.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ths.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ceh.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nmh.guannengcc.top

[L04] 设置超时
来源：http://lzz.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://mgr.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jgz.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfv.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://llu.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zsv.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rea.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fcx.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fmu.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://jui.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rxy.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nww.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pgj.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wzt.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tkw.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mfv.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mpf.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zcg.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://wpq.fanxiaobao.xyz

Py:   resp.json()
来源：http://qzf.daria6918.cn

PHP:  json_decode($body, true);
来源：http://mva.9152youxi.cn

JS:   await resp.json()
来源：http://wkp.hcnkem.com

TS:   await resp.json()
来源：http://hdn.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uxn.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oks.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://lgi.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gel.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://glm.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ijy.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://est.yongpay.top

JS:   resp.ok;  resp.status
来源：http://kwx.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://igc.wangdashe.top

Java: resp.statusCode()
来源：http://rll.c1oappe.top

Go:   resp.StatusCode
来源：http://quv.yvedp.cn

Ruby: resp.code.to_i
来源：http://bzf.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://wum.cdnleiting.top

[L08] 并发请求多个地址
来源：http://nvb.fktsv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mou.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://fue.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lma.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vyh.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tfm.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fad.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vms.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ysc.yj20258888.top

================================================================================
来源：http://lmz.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://cdj.yanxiufei.cn

================================================================================
来源：http://nlc.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://ras.yj20258.top

Py:   sys.argv[1:]
来源：http://nfx.tanke756.top

PHP:  $argv;  $argc;
来源：http://hgl.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://jar.xingfuxueyuan.xyz

TS:   process.argv.slice(2)
来源：http://yno.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://rfi.cashguo.top

Go:   os.Args[1:]
来源：http://xqj.sxryk.cn

Ruby: ARGV
来源：http://kus.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://ktk.kuanghao11.cn

[M02] 读取环境变量
来源：http://ykg.meibo888.top

Py:   os.environ.get("HOME")
来源：http://dvr.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eix.xziqi.cn

JS:   process.env.HOME
来源：http://vwi.jqgfzy.top

TS:   process.env.HOME
来源：http://pyd.birdmap.top

Java: System.getenv("HOME")
来源：http://wuf.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xzq.yvedp.cn

Ruby: ENV["HOME"]
来源：http://war.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lfn.fehbvm.com

[M03] 执行外部命令
来源：http://whn.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ouv.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lqq.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xsm.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://jcs.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jqf.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://giy.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://ntp.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://uzf.redwolf501.top

[M04] 获取当前工作目录
来源：http://fsg.yfazqb.com

Py:   os.getcwd()
来源：http://cqu.shuidangran.top

PHP:  getcwd();
来源：http://wwx.ehwqpu.com

JS:   process.cwd()
来源：http://jpa.ehwqpu.com

TS:   process.cwd()
来源：http://zct.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://uss.xuetiantiany.cn

Go:   os.Getwd()
来源：http://gze.redwolf501.top

Ruby: Dir.pwd
来源：http://yjs.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://zqa.c1oappe.top

[M05] 设置退出码
来源：http://bev.fengsongda.top

Py:   sys.exit(1)
来源：http://aah.yangfankeji.com

PHP:  exit(1);
来源：http://ucq.yj20258888.top

JS:   process.exit(1)
来源：http://wdu.shangyingyoupin.top

TS:   process.exit(1)
来源：http://gjg.ehwqpu.com

Java: System.exit(1)
来源：http://ioy.kuanghao11.cn

Go:   os.Exit(1)
来源：http://brp.zycfv.cn

Ruby: exit 1
来源：http://wvs.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ovf.yanxiufei.cn

[M06] 向标准错误输出
来源：http://pfv.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://zaq.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://flg.uphjek.com

JS:   console.error("err")
来源：http://slu.gogol.net.cn

TS:   console.error("err")
来源：http://dcw.haohaochexian.top

Java: System.err.println("err")
来源：http://cbe.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://foa.jinghuilouyu.cn

Ruby: warn "err"
来源：http://thq.ppjwa.cn

C#:   Console.Error.WriteLine("err")
来源：http://iee.daxiang520.top

[M07] 判断是否为主入口
来源：http://jsx.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://wca.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pof.yj20258888.top

JS:   require.main === module
来源：http://obb.cucudq.cn

TS:   require.main === module
来源：http://igy.fzhhl.top

Java: public static void main(String[] args)
来源：http://zte.yj202588.top

Go:   func main()
来源：http://gxw.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kuf.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://ogv.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://qfk.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://fhz.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://tmk.ppjwa.cn

JS:   process.platform;  process.version
来源：http://lzv.uphjek.com

TS:   process.platform;  process.version
来源：http://irp.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lyh.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rzp.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mpy.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kqq.yfazqb.com

================================================================================
来源：http://fxw.shuidangran.top

N. 数据结构与算法
来源：http://rul.zhixingplan.top

================================================================================
来源：http://vmr.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://omk.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://jrv.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xwk.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yey.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lef.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://ncl.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://keq.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vda.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wua.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://alu.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://gck.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aiy.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xsn.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tky.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wml.shuidangran.top

Go:   slices.Sort(arr)
来源：http://fzi.yj20258.top

Ruby: arr.sort
来源：http://qja.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vwg.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://ibs.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ppj.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://zzn.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oek.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://euy.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ibh.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blr.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zvu.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://gon.gotoacloud.top

[N04] 斐波那契数列
来源：http://ffw.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cuu.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eet.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vko.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gba.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vvi.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://skc.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rkg.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kcu.bjfxy.top

[N05] 最大公约数
来源：http://zmo.yonumen.top

Py:   math.gcd(a, b)
来源：http://ajv.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ghr.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zgq.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ewa.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hkv.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bma.yangfankeji.com

Ruby: a.gcd(b)
来源：http://knu.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rah.haohaochexian.top

[N06] 判断回文字符串
来源：http://vyu.sxryk.cn

Py:   s == s[::-1]
来源：http://jar.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://ppq.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://ojx.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://imb.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lgs.yvedp.cn

Go:   // 双指针从两端比较
来源：http://agi.cashguo.top

Ruby: s == s.reverse
来源：http://zbc.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lmt.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://xjk.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://afm.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kks.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fjy.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://dcj.chenzaomai.com

Java: // 手写 HashMap
来源：http://mfu.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://tpl.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://ytf.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://tbt.ppjwa.cn

[N08] 生成全排列
来源：http://ntf.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://ata.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://ebs.xziqi.cn

JS:   // 手写回溯递归
来源：http://tzx.redwolf501.top

TS:   // 手写回溯递归
来源：http://tak.epnwcf.com

Java: // 手写回溯递归
来源：http://lhz.fengsongda.top

Go:   // 手写回溯递归
来源：http://pjf.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://iqo.zycfv.cn

C#:   // 手写回溯递归
来源：http://eya.vehdjk.com

[N09] 栈与队列
来源：http://mbr.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lvr.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ruq.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mav.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cev.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://juy.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pzf.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cdo.wangshuangyany.cn


<!-- 参考信息 -->