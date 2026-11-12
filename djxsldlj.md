代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kgb.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fpo.meibo888.top

JS:   JSON.stringify(obj)
来源：http://dmt.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://xfv.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lpk.uphjek.com

Go:   json.Marshal(obj)
来源：http://hug.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://zqv.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hbw.mhx1999.top

[K02] JSON 字符串转对象
来源：http://fub.ydzc1.top

Py:   json.loads(s)
来源：http://gnc.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rhj.yonumen.top

JS:   JSON.parse(s)
来源：http://iey.xziqi.cn

TS:   JSON.parse(s)
来源：http://vai.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hbb.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://avf.gzhubu.top

Ruby: JSON.parse(s)
来源：http://phm.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://efl.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://hde.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://alf.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uis.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://szx.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lis.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sjd.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cco.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://yaq.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nti.smart0.xyz

[K04] 读取 JSON 文件
来源：http://ufn.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ets.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jvm.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://afq.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vfp.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qnc.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lbe.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://hxm.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nos.aizwys.cn

[K05] 深拷贝对象
来源：http://yqh.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://ycb.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://clz.wangdashe.top

JS:   structuredClone(obj)
来源：http://yok.gogol.net.cn

TS:   structuredClone(obj)
来源：http://ukc.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qbl.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://afp.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bvb.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hop.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://tkq.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yfl.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uem.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://utt.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwn.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eqg.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rmg.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wwe.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://psw.vehdjk.com

[K07] 进制转换
来源：http://zha.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mzq.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fae.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wzu.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://huq.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mzl.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wiw.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zmc.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://ggi.ivvv.top

Py:   pickle.dumps(obj)
来源：http://iws.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jpl.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://koz.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://zjx.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ocf.nwbrower.top

Go:   encoding/gob
来源：http://epv.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://ivo.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://awr.epnwcf.com

================================================================================
来源：http://obl.ydjk.org.cn

L. 网络请求
来源：http://gcy.shangyingyoupin.top

================================================================================
来源：http://hwe.zdqjudy.top

[L01] 发送 GET 请求
来源：http://xvc.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mrh.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hjh.quarkkingdee.top

JS:   await fetch(url)
来源：http://xpf.nanxinkj.top

TS:   await fetch(url)
来源：http://sde.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://abq.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://svw.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://alw.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ugj.yueranfly.top

[L02] 发送 POST JSON
来源：http://esv.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://hhe.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yxl.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://raj.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eer.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eie.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ogw.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lkb.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kwv.hesvh.cn

[L03] 设置自定义请求头
来源：http://qbn.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nzv.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iub.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://atw.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bun.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://snj.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jzj.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rdr.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://que.havefunace.top

[L04] 设置超时
来源：http://nyu.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://vtl.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ehs.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cfx.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dzy.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gzd.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nea.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sbm.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iej.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://jug.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tpq.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://afv.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kja.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://who.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lav.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fyq.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lgs.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iwd.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://cke.wangdashe.top

Py:   resp.json()
来源：http://qxd.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://qay.bbcook.cn

JS:   await resp.json()
来源：http://toj.jinqigfzy.top

TS:   await resp.json()
来源：http://gds.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cri.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lzy.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://nfs.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wky.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://rhz.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bsa.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bcm.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://qco.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://nte.daxiang520.top

Java: resp.statusCode()
来源：http://ryx.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://ncl.smart0.xyz

Ruby: resp.code.to_i
来源：http://igs.yj202588.top

C#:   (int)resp.StatusCode
来源：http://pab.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://tgg.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pgb.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://sim.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mqa.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qwa.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fwk.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rbw.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jfn.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jqm.fanxiaobao.xyz

================================================================================
来源：http://neg.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://pfa.fzhhl.top

================================================================================
来源：http://seo.sufxvd.cn

[M01] 读取命令行参数
来源：http://oph.wangdashe.top

Py:   sys.argv[1:]
来源：http://doy.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://tfd.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://qhx.yj202588.top

TS:   process.argv.slice(2)
来源：http://cvm.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://rjl.zycfv.cn

Go:   os.Args[1:]
来源：http://niq.ppjwa.cn

Ruby: ARGV
来源：http://fef.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://awa.ydzc1.top

[M02] 读取环境变量
来源：http://ikp.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://tdz.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wfr.sweek.top

JS:   process.env.HOME
来源：http://kqw.yonumen.top

TS:   process.env.HOME
来源：http://ifr.nanxuanxn.top

Java: System.getenv("HOME")
来源：http://tpf.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mjy.iojbl.cn

Ruby: ENV["HOME"]
来源：http://qxw.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oiu.jqgufenzy.top

[M03] 执行外部命令
来源：http://byp.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fhz.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fyi.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tcq.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ley.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kmx.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nlv.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yer.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://zdr.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://rsc.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://arq.havefunace.top

PHP:  getcwd();
来源：http://bmm.mhx1999.top

JS:   process.cwd()
来源：http://ezp.ivvv.top

TS:   process.cwd()
来源：http://dsi.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://zho.zdbjq.cn

Go:   os.Getwd()
来源：http://uko.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://sis.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gzl.quarkkingdee.top

[M05] 设置退出码
来源：http://isc.bbcook.cn

Py:   sys.exit(1)
来源：http://jvt.ppjwa.cn

PHP:  exit(1);
来源：http://ubz.ydjk.org.cn

JS:   process.exit(1)
来源：http://wmh.haohaochexian.top

TS:   process.exit(1)
来源：http://cyq.xziqi.cn

Java: System.exit(1)
来源：http://taa.52xcode.cn

Go:   os.Exit(1)
来源：http://pyv.shangyingyoupin.top

Ruby: exit 1
来源：http://oza.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ixv.uphjek.com

[M06] 向标准错误输出
来源：http://zuw.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://ldp.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lto.bjfxy.top

JS:   console.error("err")
来源：http://fqq.iojbl.cn

TS:   console.error("err")
来源：http://ilg.yangfankeji.com

Java: System.err.println("err")
来源：http://vcz.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sdv.fzhhl.top

Ruby: warn "err"
来源：http://svy.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://upz.fktsv.cn

[M07] 判断是否为主入口
来源：http://toh.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://fqc.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qcx.fengsongda.top

JS:   require.main === module
来源：http://zqi.smart0.xyz

TS:   require.main === module
来源：http://fhn.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://gjf.fehbvm.com

Go:   func main()
来源：http://pcu.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dsq.yonumen.top

C#:   static void Main(string[] args)
来源：http://rad.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://igu.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://tsj.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://itt.hammf.cn

JS:   process.platform;  process.version
来源：http://aih.sysykeji.top

TS:   process.platform;  process.version
来源：http://dot.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xcs.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cqd.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ecp.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://otc.chenlongwang.top

================================================================================
来源：http://xep.cucudq.cn

N. 数据结构与算法
来源：http://ncd.birdmap.top

================================================================================
来源：http://wkk.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://hve.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://njk.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hup.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oby.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iet.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://xsr.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://iff.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hfg.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://sam.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://ofi.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://dek.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gia.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xnc.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fne.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oua.jianghu66.top

Go:   slices.Sort(arr)
来源：http://ett.jiagoushi.top

Ruby: arr.sort
来源：http://xfp.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qtz.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://lno.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tpi.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://mzx.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qvb.fktsv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://trs.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://faw.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ieh.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wzq.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://cbs.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://sjn.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hml.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qfa.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pbn.fehbvm.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dan.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blj.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iva.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hei.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vzc.aizwys.cn

[N05] 最大公约数
来源：http://eva.redwolf501.top

Py:   math.gcd(a, b)
来源：http://ydn.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rdk.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kja.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aur.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nvu.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lmg.epnwcf.com

Ruby: a.gcd(b)
来源：http://tjl.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://api.yueranfly.top

[N06] 判断回文字符串
来源：http://jbe.yongpay.top

Py:   s == s[::-1]
来源：http://csf.guannengcc.top

PHP:  $s === strrev($s);
来源：http://fal.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://xfm.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://fve.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kte.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://hny.fktsv.cn

Ruby: s == s.reverse
来源：http://xkn.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mws.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://xwe.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vew.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rzx.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://liv.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://qwf.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://gab.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://pdk.hesvh.cn

Ruby: // 手写 Hash
来源：http://usi.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://kix.cqqwz.cn

[N08] 生成全排列
来源：http://uty.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://qai.ybcxt.top

PHP:  // 手写递归交换
来源：http://wen.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://dpe.cdnleiting.top

TS:   // 手写回溯递归
来源：http://wdt.hnxiangtu.top

Java: // 手写回溯递归
来源：http://pju.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://dol.havefunace.top

Ruby: arr.permutation.to_a
来源：http://uov.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://krq.chenlongwang.top

[N09] 栈与队列
来源：http://nut.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://see.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dgs.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://glr.tian-w.cn


<!-- 参考信息 -->