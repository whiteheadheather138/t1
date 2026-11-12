代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rzy.xylfe.cn

Go:   json.Marshal(obj)
来源：http://bjy.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ncz.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://jhs.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://rdd.yueranfly.top

Py:   json.loads(s)
来源：http://kek.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://did.hnqzz.top

JS:   JSON.parse(s)
来源：http://wui.0kj1m.cn

TS:   JSON.parse(s)
来源：http://yge.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://odp.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://lov.tian-w.cn

Ruby: JSON.parse(s)
来源：http://cxy.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fby.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://zyr.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://isb.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jpv.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://tha.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://avl.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nkv.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://paz.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wzi.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lat.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://nee.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://orx.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yyl.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cmi.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pwc.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nek.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://chd.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://orp.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://opn.ctjpmb.com

[K05] 深拷贝对象
来源：http://ksz.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://qoa.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://xzo.hesvh.cn

JS:   structuredClone(obj)
来源：http://uoe.yuxming.cn

TS:   structuredClone(obj)
来源：http://pmu.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jwc.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vha.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vlp.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lrg.tarul.cn

[K06] 解析 URL 查询串
来源：http://rxk.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xyv.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yqd.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cri.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lqa.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vbm.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kxb.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jgv.zhengqikj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tjp.fehbvm.com

[K07] 进制转换
来源：http://efq.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kgm.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hxw.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ebx.yj20258.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ytv.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qiv.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ycv.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bzo.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lts.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://iav.cashguo.top

Py:   pickle.dumps(obj)
来源：http://kup.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mfs.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://wbi.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://qou.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cuu.tian-w.cn

Go:   encoding/gob
来源：http://soy.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://szn.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ssw.yfazqb.com

================================================================================
来源：http://wba.zhongyouzk.top

L. 网络请求
来源：http://ohk.ydzc1.top

================================================================================
来源：http://fku.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://tqy.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ngx.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nun.ivvv.top

JS:   await fetch(url)
来源：http://zmq.chenzaomai.com

TS:   await fetch(url)
来源：http://jww.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tlf.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://ggg.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://eoz.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xfr.smart0.xyz

[L02] 发送 POST JSON
来源：http://myz.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://aro.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://coy.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ojd.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wmw.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wzm.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://owz.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kys.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jlr.mhx1999.top

[L03] 设置自定义请求头
来源：http://tkz.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zbl.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://poh.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://noc.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://heq.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mpw.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ebj.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jaw.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ctg.vqdsnc.cn

[L04] 设置超时
来源：http://bgq.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://psx.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://law.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sxx.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ags.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://laz.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qng.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fxa.havefunace.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hbx.fengsongda.top

[L05] 上传文件（multipart）
来源：http://qgp.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://niz.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ycv.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dab.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pjt.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wlg.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vvl.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lvg.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zeu.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://tex.yj202588.top

Py:   resp.json()
来源：http://akh.yj202588.top

PHP:  json_decode($body, true);
来源：http://dso.shuidangran.top

JS:   await resp.json()
来源：http://wxx.shzxlz.cn

TS:   await resp.json()
来源：http://vlm.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qbl.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nol.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://itn.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cbx.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://sfy.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qwu.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hdn.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://ajc.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://eyv.wangshuangyany.cn

Java: resp.statusCode()
来源：http://khq.xziqi.cn

Go:   resp.StatusCode
来源：http://aex.fehbvm.com

Ruby: resp.code.to_i
来源：http://cpl.ctjpmb.com

C#:   (int)resp.StatusCode
来源：http://feh.hysaishi.cn

[L08] 并发请求多个地址
来源：http://zsu.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cpt.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://hkd.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zfn.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xlb.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nfv.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kfk.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aiu.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xom.meibo888.top

================================================================================
来源：http://gsk.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://pzg.hcnkem.com

================================================================================
来源：http://upc.zhixingplan.top

[M01] 读取命令行参数
来源：http://ogw.yuanzhike.top

Py:   sys.argv[1:]
来源：http://oip.smart0.xyz

PHP:  $argv;  $argc;
来源：http://xzq.c1oappe.top

JS:   process.argv.slice(2)
来源：http://kgp.fehbvm.com

TS:   process.argv.slice(2)
来源：http://jff.cashguo.top

Java: args 数组（main 方法参数）
来源：http://bls.jqgfzy.top

Go:   os.Args[1:]
来源：http://oln.sjlbkw.cn

Ruby: ARGV
来源：http://wlp.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://fsx.yj20258.top

[M02] 读取环境变量
来源：http://xhy.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://ysb.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lir.yj20258.top

JS:   process.env.HOME
来源：http://ttf.kuanghao11.cn

TS:   process.env.HOME
来源：http://vsa.iojbl.cn

Java: System.getenv("HOME")
来源：http://kua.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ueb.nanxuanxn.top

Ruby: ENV["HOME"]
来源：http://fed.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://seu.xziqi.cn

[M03] 执行外部命令
来源：http://lci.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ont.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://emx.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aks.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://efd.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://owr.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://iel.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://him.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://xsl.dashuyun.cn

[M04] 获取当前工作目录
来源：http://vzv.yangfankeji.com

Py:   os.getcwd()
来源：http://jzp.daxiang520.top

PHP:  getcwd();
来源：http://jcb.jinqigfzy.top

JS:   process.cwd()
来源：http://rmh.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://lyo.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://spa.daxiang520.top

Go:   os.Getwd()
来源：http://ayk.jlsjyb.cn

Ruby: Dir.pwd
来源：http://eln.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://vis.feifeiyinyue.top

[M05] 设置退出码
来源：http://lix.nanxuanxn.top

Py:   sys.exit(1)
来源：http://fnr.svipenyu.cn

PHP:  exit(1);
来源：http://huc.iojbl.cn

JS:   process.exit(1)
来源：http://zjf.tarul.cn

TS:   process.exit(1)
来源：http://ydf.zycfv.cn

Java: System.exit(1)
来源：http://zrr.yonumen.top

Go:   os.Exit(1)
来源：http://rkm.sweek.top

Ruby: exit 1
来源：http://zrc.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ohw.hcnkem.com

[M06] 向标准错误输出
来源：http://wio.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://bvw.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://mra.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://pgs.sxryk.cn

TS:   console.error("err")
来源：http://grn.smart0.xyz

Java: System.err.println("err")
来源：http://kln.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fwb.pengpengdd.cyou

Ruby: warn "err"
来源：http://qjj.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://wkm.yonumen.top

[M07] 判断是否为主入口
来源：http://pai.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://pkb.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wuk.iojbl.cn

JS:   require.main === module
来源：http://duj.hcnkem.com

TS:   require.main === module
来源：http://brs.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://sza.kuanghao11.cn

Go:   func main()
来源：http://hwq.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qjv.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://sig.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://igj.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://lsy.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://zdz.yj202588.top

JS:   process.platform;  process.version
来源：http://ybc.cqqwz.cn

TS:   process.platform;  process.version
来源：http://pkl.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://szl.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mow.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eiz.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://vzc.ppjwa.cn

================================================================================
来源：http://iol.wangshuangyany.cn

N. 数据结构与算法
来源：http://zcv.chenlongwang.top

================================================================================
来源：http://yoq.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://aev.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dah.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://arb.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mqv.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://upd.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lbu.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://dyi.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kdv.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lxa.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://vcy.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://lsy.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dzx.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eeo.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://wgj.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wen.nwbrower.top

Go:   slices.Sort(arr)
来源：http://tjh.316326.xyz

Ruby: arr.sort
来源：http://gkx.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ixg.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://ynj.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yxj.ywan-chungtsiang.top

PHP:  // 递归实现，或用 usort
来源：http://tpw.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://efc.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oeh.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vav.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ubx.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lzd.quarkkingdee.top

C#:   // 手写递归，或 Array.Sort
来源：http://rsg.fehbvm.com

[N04] 斐波那契数列
来源：http://vas.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wgv.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ahm.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qdf.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gjc.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tkq.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qwa.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dbs.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vzj.zhixingplan.top

[N05] 最大公约数
来源：http://ltx.daxiang520.top

Py:   math.gcd(a, b)
来源：http://gqq.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hjl.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cvi.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fmx.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cae.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mjo.pycfn.com

Ruby: a.gcd(b)
来源：http://ask.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kkg.bbcook.cn

[N06] 判断回文字符串
来源：http://ash.nwbrower.top

Py:   s == s[::-1]
来源：http://vbu.andypj.xyz

PHP:  $s === strrev($s);
来源：http://nyf.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://elv.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://dzk.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yag.xylfe.cn

Go:   // 双指针从两端比较
来源：http://rjf.yj20258.top

Ruby: s == s.reverse
来源：http://gln.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rmc.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://okk.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fby.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wny.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nus.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://qbo.ydzc1.top

Java: // 手写 HashMap
来源：http://gfq.havefunace.top

Go:   // 手写 map[int]int
来源：http://out.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://uie.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://xss.ppjwa.cn

[N08] 生成全排列
来源：http://acm.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://zlw.shzxlz.cn

PHP:  // 手写递归交换
来源：http://bit.zdbjq.cn

JS:   // 手写回溯递归
来源：http://xvy.yfazqb.com

TS:   // 手写回溯递归
来源：http://fko.yangfankeji.com

Java: // 手写回溯递归
来源：http://ovv.svipenyu.cn

Go:   // 手写回溯递归
来源：http://tda.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://cqo.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://jcb.sxryk.cn

[N09] 栈与队列
来源：http://kwz.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://alp.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uzy.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eji.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eoi.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://thv.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rla.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://onm.cashguo.top


<!-- 参考信息 -->