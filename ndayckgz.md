代发 wailian999

[K02] JSON 字符串转对象
来源：http://mem.fktsv.cn

Py:   json.loads(s)
来源：http://sck.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zqo.gotoacloud.top

JS:   JSON.parse(s)
来源：http://diy.haohaochexian.top

TS:   JSON.parse(s)
来源：http://lzp.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hjk.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://lhk.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://nrl.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ysv.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://sbj.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yaq.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jld.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tql.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://opy.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bvn.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ujb.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dil.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jwq.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://pzs.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lcd.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pkl.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpj.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fuq.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zpd.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blc.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nyn.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yez.vehdjk.com

[K05] 深拷贝对象
来源：http://ibi.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://srz.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://ysu.gotoacloud.top

JS:   structuredClone(obj)
来源：http://arg.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://gqn.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://drm.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rcz.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ezd.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xho.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://gcd.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qiz.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nee.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://exy.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mjv.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ldi.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://czm.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fxq.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ktj.nanxuanxn.top

[K07] 进制转换
来源：http://xdd.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://snm.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sup.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pmb.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iyz.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pay.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ruk.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wgo.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://atb.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://eeo.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://sqr.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sws.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://wma.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://rqy.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mft.yanxiufei.cn

Go:   encoding/gob
来源：http://tzt.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://owq.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tar.zhaomingkeji.xyz

================================================================================
来源：http://aci.zhijiandao.cn

L. 网络请求
来源：http://xzv.dashuyun.cn

================================================================================
来源：http://oxb.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://zrd.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dni.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hud.meibo888.top

JS:   await fetch(url)
来源：http://hrw.xuanzx.com

TS:   await fetch(url)
来源：http://fdv.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ulv.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://jsm.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://puq.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hwf.jinqigufen.top

[L02] 发送 POST JSON
来源：http://cua.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://pmo.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cdv.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aiy.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fxl.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sci.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ymp.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tcb.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qmz.tarul.cn

[L03] 设置自定义请求头
来源：http://uyb.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qem.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rbu.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mnt.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sdx.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mkt.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iuz.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jan.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wbv.yonumen.top

[L04] 设置超时
来源：http://avi.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://bew.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://onx.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eyy.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dpz.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bxa.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ofq.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zzb.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hot.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://tbh.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oah.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kdy.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://btc.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pek.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gxm.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pbz.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jty.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bkl.yfazqb.com

[L06] 解析响应为 JSON
来源：http://ehf.52xcode.cn

Py:   resp.json()
来源：http://mjx.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://mnj.yuanzhike.top

JS:   await resp.json()
来源：http://tft.fzhhl.top

TS:   await resp.json()
来源：http://bji.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ffw.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kyy.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://gkh.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oqn.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://lwy.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eis.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jws.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://rmu.hammf.cn

TS:   resp.ok;  resp.status
来源：http://ypo.shuidangran.top

Java: resp.statusCode()
来源：http://drk.zdbjq.cn

Go:   resp.StatusCode
来源：http://glg.hysaishi.cn

Ruby: resp.code.to_i
来源：http://bot.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://bnx.9152youxi.cn

[L08] 并发请求多个地址
来源：http://xiv.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kzc.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://mgt.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://usr.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwb.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zyp.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mzt.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kfl.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dat.fktsv.cn

================================================================================
来源：http://yzr.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://qtp.ctjpmb.com

================================================================================
来源：http://nuo.cdnleiting.top

[M01] 读取命令行参数
来源：http://nnf.meibo888.top

Py:   sys.argv[1:]
来源：http://ofy.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://yuy.yvedp.cn

JS:   process.argv.slice(2)
来源：http://ydm.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://irr.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://kwx.jqgufenzy.top

Go:   os.Args[1:]
来源：http://srg.jinyuanbaomall.cn

Ruby: ARGV
来源：http://zgq.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://zqp.guannengcc.top

[M02] 读取环境变量
来源：http://ups.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://mgw.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sol.xziqi.cn

JS:   process.env.HOME
来源：http://gib.cheryme.top

TS:   process.env.HOME
来源：http://soa.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://cap.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bzo.jianghu66.top

Ruby: ENV["HOME"]
来源：http://urt.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xoh.tianlin.xyz

[M03] 执行外部命令
来源：http://kjp.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lww.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://opk.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://shp.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://vyl.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nds.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tmt.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://ene.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://yqb.bjfxy.top

[M04] 获取当前工作目录
来源：http://csj.tanke756.top

Py:   os.getcwd()
来源：http://gby.zhiwuduotai.top

PHP:  getcwd();
来源：http://clt.zhongyouzk.top

JS:   process.cwd()
来源：http://kyz.hnqzz.top

TS:   process.cwd()
来源：http://fno.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://upz.hongshengwenyu.top

Go:   os.Getwd()
来源：http://wvf.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://kum.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kuz.redwolf501.top

[M05] 设置退出码
来源：http://mbt.yvedp.cn

Py:   sys.exit(1)
来源：http://llh.cdnleiting.top

PHP:  exit(1);
来源：http://vsa.kuanghao11.cn

JS:   process.exit(1)
来源：http://koo.jqgfzy.top

TS:   process.exit(1)
来源：http://aaw.daxiang520.top

Java: System.exit(1)
来源：http://gbu.316326.xyz

Go:   os.Exit(1)
来源：http://wbp.wangdashe.top

Ruby: exit 1
来源：http://jrn.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://omk.havefunace.top

[M06] 向标准错误输出
来源：http://cfh.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://jqi.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xfx.sweek.top

JS:   console.error("err")
来源：http://gwt.yj202588.top

TS:   console.error("err")
来源：http://vkv.zhongyouzk.top

Java: System.err.println("err")
来源：http://ajq.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sdf.nwbrower.top

Ruby: warn "err"
来源：http://rkn.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://wfp.cashguo.top

[M07] 判断是否为主入口
来源：http://nnm.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://xyl.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oct.guowangkeji.top

JS:   require.main === module
来源：http://ssw.zhaomingkeji.xyz

TS:   require.main === module
来源：http://jgg.shuidangran.top

Java: public static void main(String[] args)
来源：http://xck.vehdjk.com

Go:   func main()
来源：http://scl.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dpo.ydzc1.top

C#:   static void Main(string[] args)
来源：http://nur.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://abq.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://jke.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://mnq.52xcode.cn

JS:   process.platform;  process.version
来源：http://cry.tianlin.xyz

TS:   process.platform;  process.version
来源：http://ryj.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wbs.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iwb.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xaj.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xgh.zdqjudy.top

================================================================================
来源：http://vmh.chenzaomai.com

N. 数据结构与算法
来源：http://pic.sjlbkw.cn

================================================================================
来源：http://dow.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://uqw.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://nud.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ubg.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://axn.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qyt.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://gqg.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://hwo.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://upf.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://vby.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://njc.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://vcq.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fej.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uid.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fjy.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fhh.daria6918.cn

Go:   slices.Sort(arr)
来源：http://vak.pycfn.com

Ruby: arr.sort
来源：http://itt.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bjq.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://rwc.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bhc.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://hxf.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ucv.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qsa.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zjc.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ehz.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aqf.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://dfq.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://dwk.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tsc.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yuv.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yih.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lcd.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jev.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://icy.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yrd.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pzi.xziqi.cn

[N05] 最大公约数
来源：http://ylr.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://zzs.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qly.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wxm.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qky.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dig.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ftn.uphjek.com

Ruby: a.gcd(b)
来源：http://vsn.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tuc.hysaishi.cn

[N06] 判断回文字符串
来源：http://jur.meibo888.top

Py:   s == s[::-1]
来源：http://mmr.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://knm.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://xww.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://wyq.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://svl.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://uyf.jqgfzy.top

Ruby: s == s.reverse
来源：http://qls.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cqa.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://oek.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jgc.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nhj.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cgc.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://zjg.nanxuanxn.top

Java: // 手写 HashMap
来源：http://mot.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://ywj.cdnleiting.top

Ruby: // 手写 Hash
来源：http://zpj.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://zao.zhiwuduotai.top

[N08] 生成全排列
来源：http://rse.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://rbw.sxryk.cn

PHP:  // 手写递归交换
来源：http://auj.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://tdr.chenzaomai.com

TS:   // 手写回溯递归
来源：http://koa.guowangkeji.top

Java: // 手写回溯递归
来源：http://orx.hcnkem.com

Go:   // 手写回溯递归
来源：http://ulp.yj20258.top

Ruby: arr.permutation.to_a
来源：http://xsz.redwolf501.top

C#:   // 手写回溯递归
来源：http://sza.birdmap.top

[N09] 栈与队列
来源：http://irb.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://krg.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://txn.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://veg.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://boh.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ynz.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ssx.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sbu.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://axs.yanxiufei.cn

[N10] 链表节点定义
来源：http://gnu.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kmr.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yws.xuetiantiany.cn


<!-- 参考信息 -->