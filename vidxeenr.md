代发 wailian999

================================================================================
来源：http://wpk.yonumen.top

K. JSON 与序列化
来源：http://yob.hongshengwenyu.top

================================================================================
来源：http://wlk.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://uab.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://piw.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lgc.sweek.top

JS:   JSON.stringify(obj)
来源：http://lpz.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://pcd.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dvl.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://nvn.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://spw.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nui.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://fgr.pengpengdd.cyou

Py:   json.loads(s)
来源：http://uad.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fjr.snrcjt.cn

JS:   JSON.parse(s)
来源：http://odc.zycfv.cn

TS:   JSON.parse(s)
来源：http://zwh.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rnr.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://lvh.shuidangran.top

Ruby: JSON.parse(s)
来源：http://ixr.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hqg.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://fzw.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nwt.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ley.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vcf.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lzg.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bnm.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dam.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rjs.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ivt.fehbvm.com

[K04] 读取 JSON 文件
来源：http://qmp.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tsk.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aqz.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cuf.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jvw.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pwf.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qei.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://bhp.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zfv.cdnleiting.top

[K05] 深拷贝对象
来源：http://mmm.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://hlj.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://pms.hammf.cn

JS:   structuredClone(obj)
来源：http://qsx.ydzc1.top

TS:   structuredClone(obj)
来源：http://xtv.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tkh.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dye.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tep.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xye.xylfe.cn

[K06] 解析 URL 查询串
来源：http://aub.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bdd.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lwb.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fqt.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpk.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://viu.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qmf.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gds.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vls.hongshengwenyu.top

[K07] 进制转换
来源：http://heu.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://udg.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dej.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xng.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uwr.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ryf.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iip.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yrv.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://riz.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://kce.yj20258.top

Py:   pickle.dumps(obj)
来源：http://vif.zhiwuduotai.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zpn.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://yvf.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://cgn.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hub.snrcjt.cn

Go:   encoding/gob
来源：http://xrp.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://cmk.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eey.mhx1999.top

================================================================================
来源：http://asi.shangyingyoupin.top

L. 网络请求
来源：http://zfv.pycfn.com

================================================================================
来源：http://tpn.tanke756.top

[L01] 发送 GET 请求
来源：http://jvk.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mol.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lcq.tianlin.xyz

JS:   await fetch(url)
来源：http://rih.0kj1m.cn

TS:   await fetch(url)
来源：http://uyb.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://byh.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://wnt.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://gkw.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hkp.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://bpk.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://kws.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kso.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pre.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zud.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fjz.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jik.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nbq.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tey.smart0.xyz

[L03] 设置自定义请求头
来源：http://yml.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://box.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jee.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnk.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xuh.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypb.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://svv.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vid.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rks.fehbvm.com

[L04] 设置超时
来源：http://lzl.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://dmh.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qkj.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eju.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vjk.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://doj.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vdm.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hnr.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zol.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://gps.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zor.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://stb.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wwj.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tpr.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jhy.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mqj.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tmu.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rcq.xinyue.icu

[L06] 解析响应为 JSON
来源：http://uip.tarul.cn

Py:   resp.json()
来源：http://mfj.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://ijg.quarkkingdee.top

JS:   await resp.json()
来源：http://yim.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://ksy.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cne.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ugl.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://onc.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gqj.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://kvf.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uwd.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rff.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://pqq.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://ktq.shzxlz.cn

Java: resp.statusCode()
来源：http://kio.kuanghao11.cn

Go:   resp.StatusCode
来源：http://xel.hammf.cn

Ruby: resp.code.to_i
来源：http://nxw.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://als.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://miq.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zwc.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://rmx.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rgd.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ofk.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://upt.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ayq.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rhs.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oar.wangshuangyany.cn

================================================================================
来源：http://dnp.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://jgv.vehdjk.com

================================================================================
来源：http://iuu.dashuyun.cn

[M01] 读取命令行参数
来源：http://yok.aizwys.cn

Py:   sys.argv[1:]
来源：http://qex.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://vrq.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://bdn.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://mav.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://oxn.fehbvm.com

Go:   os.Args[1:]
来源：http://eqk.dianchejie.cn

Ruby: ARGV
来源：http://bsi.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://mrm.sxryk.cn

[M02] 读取环境变量
来源：http://two.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://gnx.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gxb.yueranfly.top

JS:   process.env.HOME
来源：http://jeu.yuanzhike.top

TS:   process.env.HOME
来源：http://bxx.fehbvm.com

Java: System.getenv("HOME")
来源：http://ihl.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cqu.tanke756.top

Ruby: ENV["HOME"]
来源：http://vlm.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jlp.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://llj.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ifd.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jhp.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xpj.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://lsz.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ifx.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mtt.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://gnf.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://iob.vehdjk.com

[M04] 获取当前工作目录
来源：http://vik.chenzaomai.com

Py:   os.getcwd()
来源：http://qwy.feifeiyinyue.top

PHP:  getcwd();
来源：http://gon.jinqigufen.top

JS:   process.cwd()
来源：http://ihk.mhx1999.top

TS:   process.cwd()
来源：http://xru.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://gab.chenlongwang.top

Go:   os.Getwd()
来源：http://rmc.cucudq.cn

Ruby: Dir.pwd
来源：http://mjx.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qzd.jianghu66.top

[M05] 设置退出码
来源：http://lsx.hesvh.cn

Py:   sys.exit(1)
来源：http://azf.shangyingyoupin.top

PHP:  exit(1);
来源：http://kpu.vqdsnc.cn

JS:   process.exit(1)
来源：http://odk.zhengqikj.top

TS:   process.exit(1)
来源：http://afi.tanke756.top

Java: System.exit(1)
来源：http://bij.jqgufenzy.top

Go:   os.Exit(1)
来源：http://duw.yj20258.top

Ruby: exit 1
来源：http://fyw.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vrg.uphjek.com

[M06] 向标准错误输出
来源：http://abx.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://xjo.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ngl.9152youxi.cn

JS:   console.error("err")
来源：http://rca.zdqjudy.top

TS:   console.error("err")
来源：http://yql.yueranfly.top

Java: System.err.println("err")
来源：http://cri.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://drp.kuanghao11.cn

Ruby: warn "err"
来源：http://daf.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://dwh.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://tzj.cashguo.top

Py:   if __name__ == "__main__":
来源：http://zuq.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eka.zhongyouzk.top

JS:   require.main === module
来源：http://zon.yanxiufei.cn

TS:   require.main === module
来源：http://gmo.yuxming.cn

Java: public static void main(String[] args)
来源：http://uhm.shangyingyoupin.top

Go:   func main()
来源：http://nzt.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://myf.fengsongda.top

C#:   static void Main(string[] args)
来源：http://vud.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://qsl.andypj.xyz

Py:   platform.system();  platform.python_version()
来源：http://cqj.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://kha.hywenlv.cn

JS:   process.platform;  process.version
来源：http://vcs.iojbl.cn

TS:   process.platform;  process.version
来源：http://ddh.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jcv.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://esd.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hsm.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://djq.jlsjyb.cn

================================================================================
来源：http://qke.zhiwuduotai.top

N. 数据结构与算法
来源：http://lne.tarul.cn

================================================================================
来源：http://xxx.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://pic.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://lvi.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dbe.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwe.fehbvm.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://daf.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://xnn.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://vli.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://ciw.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://bih.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://dgr.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://pyv.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ikz.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://snc.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rre.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://amd.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://mfy.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://lku.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xqt.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://sut.yj20258.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nwy.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://yge.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fre.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nhr.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hje.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iit.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fes.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://twf.yuanzhike.top

[N04] 斐波那契数列
来源：http://sxi.ybcxt.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ljl.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gmr.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkq.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qny.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://utn.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eul.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xmn.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://byv.snrcjt.cn

[N05] 最大公约数
来源：http://pyq.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://dtf.havefunace.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lpx.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qlk.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zis.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aqo.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hnn.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://ywb.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gfo.xylfe.cn

[N06] 判断回文字符串
来源：http://esh.xinyue.icu

Py:   s == s[::-1]
来源：http://ibm.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://cnq.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://ffd.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://njc.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lwk.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://avc.tianlin.xyz

Ruby: s == s.reverse
来源：http://vqe.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wou.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://blb.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wtp.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://phh.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lba.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://rcg.cdnleiting.top

Java: // 手写 HashMap
来源：http://rmk.yfazqb.com

Go:   // 手写 map[int]int
来源：http://atu.ybcxt.top

Ruby: // 手写 Hash
来源：http://txa.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://brm.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://pgv.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://umj.shuidangran.top

PHP:  // 手写递归交换
来源：http://izd.andypj.xyz

JS:   // 手写回溯递归
来源：http://iyv.havefunace.top

TS:   // 手写回溯递归
来源：http://dbg.sxryk.cn

Java: // 手写回溯递归
来源：http://vak.shuidangran.top

Go:   // 手写回溯递归
来源：http://vse.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://pyd.vehdjk.com

C#:   // 手写回溯递归
来源：http://fzc.ybcxt.top


<!-- 参考信息 -->