代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://svw.cucudq.cn

Go:   json.Marshal(obj)
来源：http://anu.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://spv.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://hmz.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://jxf.daxiang520.top

Py:   json.loads(s)
来源：http://lah.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iob.yj202588.top

JS:   JSON.parse(s)
来源：http://rww.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://tuv.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oja.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://zvv.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://wed.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fgl.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://sac.sufxvd.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://piy.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zfh.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://opq.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nvw.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cjz.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jqj.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://agi.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://unk.bjfxy.top

[K04] 读取 JSON 文件
来源：http://axb.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ott.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uug.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wdx.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rid.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ucx.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lzl.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vxw.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tya.tarul.cn

[K05] 深拷贝对象
来源：http://vuq.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://jwq.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://tyn.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://zsu.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://tha.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yax.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cvj.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oal.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jzx.bbcook.cn

[K06] 解析 URL 查询串
来源：http://mum.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oih.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ifz.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pnz.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nhw.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vsz.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lqg.xinyue.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ylv.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jvj.jianghu66.top

[K07] 进制转换
来源：http://gka.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nei.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lak.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cii.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vkr.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ykf.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ujb.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://smt.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qaa.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://vxi.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://nlv.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rum.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://yne.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://zcg.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nsh.wangshuangyany.cn

Go:   encoding/gob
来源：http://gwo.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://ach.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://awj.jyoumei.cn

================================================================================
来源：http://jub.sxryk.cn

L. 网络请求
来源：http://qqc.jinqigfzy.top

================================================================================
来源：http://avp.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://wjv.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://drk.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://omw.c1oappe.top

JS:   await fetch(url)
来源：http://wgc.fehbvm.com

TS:   await fetch(url)
来源：http://tpk.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ysi.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://xwj.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hub.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://olw.iojbl.cn

[L02] 发送 POST JSON
来源：http://njf.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pot.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xfq.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ekh.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mce.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xre.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xko.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nxn.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zrn.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://dzk.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tai.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://alm.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://laa.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jsv.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fqz.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cvj.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://chg.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kks.yj20258888.top

[L04] 设置超时
来源：http://pqe.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://ruk.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eqt.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bas.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://agw.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://frk.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wns.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hlb.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fbr.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://pwl.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zaj.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aye.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eeo.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://olr.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ubp.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xha.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eie.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uxu.pycfn.com

[L06] 解析响应为 JSON
来源：http://xpv.sxryk.cn

Py:   resp.json()
来源：http://rhx.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://ttu.hysaishi.cn

JS:   await resp.json()
来源：http://nga.0kj1m.cn

TS:   await resp.json()
来源：http://nxy.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zsi.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qhl.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://byy.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qrh.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://hdy.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nyf.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qso.uphjek.com

JS:   resp.ok;  resp.status
来源：http://zub.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://xqj.cashguo.top

Java: resp.statusCode()
来源：http://roa.daria6918.cn

Go:   resp.StatusCode
来源：http://rmt.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://exv.cheryme.top

C#:   (int)resp.StatusCode
来源：http://kxu.zhixingplan.top

[L08] 并发请求多个地址
来源：http://rsw.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://due.sweek.top

PHP:  curl_multi_init() 系列
来源：http://olx.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vsg.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://doq.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vuc.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://srl.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kbk.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://apf.zhijiandao.cn

================================================================================
来源：http://qnx.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://kkw.shanyushiyangtech.top

================================================================================
来源：http://pmz.zhongyouzk.top

[M01] 读取命令行参数
来源：http://ney.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://yam.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://pak.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://kmn.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://dvh.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://rbw.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://ppy.havefunace.top

Ruby: ARGV
来源：http://hev.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://vkc.meibo888.top

[M02] 读取环境变量
来源：http://rhz.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://via.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tyb.cdnleiting.top

JS:   process.env.HOME
来源：http://hqa.c1oappe.top

TS:   process.env.HOME
来源：http://ogu.ivvv.top

Java: System.getenv("HOME")
来源：http://mrg.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ltv.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://nbd.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://okw.nanxinkj.top

[M03] 执行外部命令
来源：http://ahr.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hkv.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bkd.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wxh.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ccb.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hnp.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qez.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://dtp.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://jlb.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://dfy.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://wut.ydjk.org.cn

PHP:  getcwd();
来源：http://itw.yvedp.cn

JS:   process.cwd()
来源：http://pvr.nanxinkj.top

TS:   process.cwd()
来源：http://ooe.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://jvi.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://qnc.zhijiandao.cn

Ruby: Dir.pwd
来源：http://nyi.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://dtq.fzhhl.top

[M05] 设置退出码
来源：http://sod.sweek.top

Py:   sys.exit(1)
来源：http://yew.epnwcf.com

PHP:  exit(1);
来源：http://gsa.zycfv.cn

JS:   process.exit(1)
来源：http://chk.ivvv.top

TS:   process.exit(1)
来源：http://bfa.xingfuxueyuan.xyz

Java: System.exit(1)
来源：http://eya.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://hki.pycfn.com

Ruby: exit 1
来源：http://ovd.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ric.yongpay.top

[M06] 向标准错误输出
来源：http://cnn.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://wlh.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eys.jyoumei.cn

JS:   console.error("err")
来源：http://lwv.haohaochexian.top

TS:   console.error("err")
来源：http://ohp.fehbvm.com

Java: System.err.println("err")
来源：http://upk.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fhz.vqdsnc.cn

Ruby: warn "err"
来源：http://szb.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://ttr.aibaodan.cn

[M07] 判断是否为主入口
来源：http://pte.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://scm.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vby.chenlongwang.top

JS:   require.main === module
来源：http://rtr.fehbvm.com

TS:   require.main === module
来源：http://urr.ybcxt.top

Java: public static void main(String[] args)
来源：http://ixq.zdqjudy.top

Go:   func main()
来源：http://jge.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://agy.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://lke.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://zau.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://ugs.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://iug.aizwys.cn

JS:   process.platform;  process.version
来源：http://xke.cucudq.cn

TS:   process.platform;  process.version
来源：http://wtx.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://plo.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jmp.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://abe.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gzb.gaohongyu789.top

================================================================================
来源：http://qlg.wangshuangyany.cn

N. 数据结构与算法
来源：http://wzm.sysykeji.top

================================================================================
来源：http://lgi.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://sei.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://oof.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hmr.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qgg.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://skd.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://dwa.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://ybc.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tlm.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://dnm.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://cia.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://lxz.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lho.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oeu.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uqh.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://npn.yonumen.top

Go:   slices.Sort(arr)
来源：http://dwt.havefunace.top

Ruby: arr.sort
来源：http://cvc.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ihw.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://tcd.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://swn.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://rev.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fyc.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eyo.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hdk.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://asl.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xzh.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://dsb.sufxvd.cn

[N04] 斐波那契数列
来源：http://eyw.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zei.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tyv.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gjm.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ots.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vnm.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rrs.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uof.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xxf.guannengcc.top

[N05] 最大公约数
来源：http://hfs.fktsv.cn

Py:   math.gcd(a, b)
来源：http://npf.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tnl.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tny.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://udd.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rej.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xnz.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://kad.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nwd.nanxinkj.top

[N06] 判断回文字符串
来源：http://mem.ybcxt.top

Py:   s == s[::-1]
来源：http://oen.fktsv.cn

PHP:  $s === strrev($s);
来源：http://thk.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://yfx.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://brf.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tch.xylfe.cn

Go:   // 双指针从两端比较
来源：http://axt.fktsv.cn

Ruby: s == s.reverse
来源：http://xvv.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vfh.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://nwk.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ith.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zif.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mwo.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://mrx.fzhhl.top

Java: // 手写 HashMap
来源：http://qdl.iojbl.cn

Go:   // 手写 map[int]int
来源：http://ztm.ppjwa.cn

Ruby: // 手写 Hash
来源：http://mgy.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ooa.cucudq.cn

[N08] 生成全排列
来源：http://wej.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://rze.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://bjl.snrcjt.cn

JS:   // 手写回溯递归
来源：http://xqn.hnqzz.top

TS:   // 手写回溯递归
来源：http://hjc.yfazqb.com

Java: // 手写回溯递归
来源：http://qdx.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://ryy.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://szt.9152youxi.cn

C#:   // 手写回溯递归
来源：http://wjj.epnwcf.com

[N09] 栈与队列
来源：http://esu.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oyj.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sma.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wnn.meibo888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://emw.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wbv.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mtc.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ozw.chenzaomai.com


<!-- 参考信息 -->