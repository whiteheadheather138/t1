代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mhd.daria6918.cn

Go:   json.Marshal(obj)
来源：http://wfz.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://odd.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vnm.yueranfly.top

[K02] JSON 字符串转对象
来源：http://nlo.ivvv.top

Py:   json.loads(s)
来源：http://fjx.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pnm.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://gph.dashuyun.cn

TS:   JSON.parse(s)
来源：http://wlj.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kxk.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://znb.hammf.cn

Ruby: JSON.parse(s)
来源：http://kcc.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pah.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://gjx.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tmy.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lgf.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iml.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eor.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ere.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qmc.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bhu.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nbo.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://hdd.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hey.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://naj.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmm.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lex.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ugd.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jyb.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://luc.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tbp.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://jkn.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://lhn.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://axx.9152youxi.cn

JS:   structuredClone(obj)
来源：http://vtf.fktsv.cn

TS:   structuredClone(obj)
来源：http://lfg.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vkw.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://epx.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eja.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pwe.birdmap.top

[K06] 解析 URL 查询串
来源：http://mrt.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cxg.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://owh.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nya.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jsh.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qbz.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xns.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pwf.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bap.yanxiufei.cn

[K07] 进制转换
来源：http://bfw.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://crg.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://itu.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zwl.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rew.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ims.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ker.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bpe.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tel.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://tnf.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://mgt.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://nzo.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://yqo.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://qzv.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pxg.xuetiantiany.cn

Go:   encoding/gob
来源：http://bpv.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://fli.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xtq.redwolf501.top

================================================================================
来源：http://xdb.mhx1999.top

L. 网络请求
来源：http://lqi.iojbl.cn

================================================================================
来源：http://tjb.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://ytn.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cru.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cdu.9152youxi.cn

JS:   await fetch(url)
来源：http://hui.wangshuangyany.cn

TS:   await fetch(url)
来源：http://req.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fqq.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://czy.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pkf.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vae.zhixingplan.top

[L02] 发送 POST JSON
来源：http://hbr.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aem.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pln.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uxy.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lcr.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://elu.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dej.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tsx.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hhx.zycfv.cn

[L03] 设置自定义请求头
来源：http://nwo.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wul.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qfi.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wfi.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oru.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gtm.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tja.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cew.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xbk.jinqigufen.top

[L04] 设置超时
来源：http://lgd.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://eiv.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pez.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cec.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://azz.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vto.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nqy.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qwg.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jfc.52xcode.cn

[L05] 上传文件（multipart）
来源：http://yrq.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gge.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://klw.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nuq.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lwl.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uml.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ynv.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dkw.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iye.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://hhu.xylfe.cn

Py:   resp.json()
来源：http://etx.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://jkf.52xcode.cn

JS:   await resp.json()
来源：http://suj.pengpengdd.cyou

TS:   await resp.json()
来源：http://fjr.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bdr.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tuc.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://bcd.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://his.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://ghi.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wos.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://itn.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://thg.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://bqh.vehdjk.com

Java: resp.statusCode()
来源：http://mpp.cucudq.cn

Go:   resp.StatusCode
来源：http://xnn.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://fwd.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://gpv.ctjpmb.com

[L08] 并发请求多个地址
来源：http://yfi.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cfs.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://cyi.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftn.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rrk.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://npf.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qoc.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zqd.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://byd.shangyingyoupin.top

================================================================================
来源：http://lje.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://tza.zhijiandao.cn

================================================================================
来源：http://xwu.tarul.cn

[M01] 读取命令行参数
来源：http://luh.cucudq.cn

Py:   sys.argv[1:]
来源：http://xgh.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://svl.xinyue.icu

JS:   process.argv.slice(2)
来源：http://xvb.fzhhl.top

TS:   process.argv.slice(2)
来源：http://mwi.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://qeh.xziqi.cn

Go:   os.Args[1:]
来源：http://wcl.xinyue.icu

Ruby: ARGV
来源：http://eje.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://jts.guowangkeji.top

[M02] 读取环境变量
来源：http://xsm.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://ehw.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vui.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://ygf.nwbrower.top

TS:   process.env.HOME
来源：http://fhy.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://wpz.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://frg.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://ynl.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jdn.uphjek.com

[M03] 执行外部命令
来源：http://jys.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hnr.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mir.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ylj.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://guv.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wkj.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xdu.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jwy.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://uld.guannengcc.top

[M04] 获取当前工作目录
来源：http://tmi.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://apm.quarkkingdee.top

PHP:  getcwd();
来源：http://rbx.hywenlv.cn

JS:   process.cwd()
来源：http://pir.xinyue.icu

TS:   process.cwd()
来源：http://tnu.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://eas.zdqjudy.top

Go:   os.Getwd()
来源：http://xqv.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://mix.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://kdy.zhongyouzk.top

[M05] 设置退出码
来源：http://yrl.c1oappe.top

Py:   sys.exit(1)
来源：http://jnw.wangdashe.top

PHP:  exit(1);
来源：http://fsd.fengsongda.top

JS:   process.exit(1)
来源：http://suk.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://ues.sufxvd.cn

Java: System.exit(1)
来源：http://xff.yj202588.top

Go:   os.Exit(1)
来源：http://huu.hammf.cn

Ruby: exit 1
来源：http://ncb.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hvu.yangfankeji.com

[M06] 向标准错误输出
来源：http://civ.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://ogy.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ect.daria6918.cn

JS:   console.error("err")
来源：http://jjk.yuanzhike.top

TS:   console.error("err")
来源：http://rpg.jqgfzy.top

Java: System.err.println("err")
来源：http://mds.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oiv.hcnkem.com

Ruby: warn "err"
来源：http://nxf.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://bdg.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://iqb.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://prz.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aur.9152youxi.cn

JS:   require.main === module
来源：http://ygn.cashguo.top

TS:   require.main === module
来源：http://soo.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://xty.daria6918.cn

Go:   func main()
来源：http://ioc.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ygi.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://kpq.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://poz.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://glv.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://olg.fengsongda.top

JS:   process.platform;  process.version
来源：http://hiq.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://lko.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zzx.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vdw.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kqv.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://pxu.svipenyu.cn

================================================================================
来源：http://zdm.wangshuangyany.cn

N. 数据结构与算法
来源：http://uza.tanke756.top

================================================================================
来源：http://kjw.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://jqs.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://ojq.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://per.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knd.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nld.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://dfs.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://zls.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cma.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rzl.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://qgu.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://qnr.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jcd.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nvp.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oct.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gxl.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://zrj.xuetiantiany.cn

Ruby: arr.sort
来源：http://bht.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iim.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://wfi.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tnb.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://aog.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://alq.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uiu.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tbb.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jny.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qow.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ute.tarul.cn

[N04] 斐波那契数列
来源：http://adz.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ksj.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nbb.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lai.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kti.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cqs.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ubn.zhiwuduotai.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owh.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pfp.hesvh.cn

[N05] 最大公约数
来源：http://acm.nwbrower.top

Py:   math.gcd(a, b)
来源：http://jep.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bge.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aoq.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zmv.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gua.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pcg.havefunace.top

Ruby: a.gcd(b)
来源：http://ztd.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eum.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://hzp.hysaishi.cn

Py:   s == s[::-1]
来源：http://aqe.316326.xyz

PHP:  $s === strrev($s);
来源：http://jgq.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://atq.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://jjs.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aad.sysykeji.top

Go:   // 双指针从两端比较
来源：http://jsc.gotoacloud.top

Ruby: s == s.reverse
来源：http://mgc.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://arw.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://osp.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zno.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rom.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pil.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://dwy.nanxuanxn.top

Java: // 手写 HashMap
来源：http://nng.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://soo.chenzaomai.com

Ruby: // 手写 Hash
来源：http://qmu.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nyz.gogol.net.cn

[N08] 生成全排列
来源：http://lrk.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://qqk.yj20258888.top

PHP:  // 手写递归交换
来源：http://rww.yueranfly.top

JS:   // 手写回溯递归
来源：http://ecl.zdbjq.cn

TS:   // 手写回溯递归
来源：http://ebw.hywenlv.cn

Java: // 手写回溯递归
来源：http://kth.cashguo.top

Go:   // 手写回溯递归
来源：http://vmr.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://blm.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://yxa.fktsv.cn

[N09] 栈与队列
来源：http://yvs.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vuh.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lwh.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nyn.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lmd.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://war.xuetiantiany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ycq.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pgo.sjlbkw.cn


<!-- 参考信息 -->