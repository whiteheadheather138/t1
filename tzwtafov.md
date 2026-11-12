代发 wailian999

[K02] JSON 字符串转对象
来源：http://tdw.fzhhl.top

Py:   json.loads(s)
来源：http://adj.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wne.hnqzz.top

JS:   JSON.parse(s)
来源：http://nhq.fengsongda.top

TS:   JSON.parse(s)
来源：http://xra.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dmx.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://qww.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://kmz.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tvo.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://bip.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mul.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qxm.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://scv.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://xvq.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gbo.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zsf.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://ysf.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cmr.zdqjudy.top

[K04] 读取 JSON 文件
来源：http://gtr.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nln.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oqn.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tiu.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cdv.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iaw.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vmc.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jxq.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fbs.chenzaomai.com

[K05] 深拷贝对象
来源：http://mkm.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://ycm.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://sbh.pycfn.com

JS:   structuredClone(obj)
来源：http://ikt.yj20258888.top

TS:   structuredClone(obj)
来源：http://ckt.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ytn.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tto.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lrd.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zeu.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://rfa.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hpu.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gkp.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://noq.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jfs.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ulm.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dgh.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tta.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wjr.fengsongda.top

[K07] 进制转换
来源：http://mug.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hqp.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://biy.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kwb.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xgh.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cgb.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xkg.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://erw.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dfc.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://qyw.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://buj.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xxn.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://bdq.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://lqk.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cpu.iojbl.cn

Go:   encoding/gob
来源：http://gsw.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://czy.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hfp.shanyushiyangkeji.top

================================================================================
来源：http://aob.jinqigfzy.top

L. 网络请求
来源：http://svj.cheryme.top

================================================================================
来源：http://dlx.jqgfzy.top

[L01] 发送 GET 请求
来源：http://idr.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gdz.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iyb.yuanzhike.top

JS:   await fetch(url)
来源：http://muk.bbcook.cn

TS:   await fetch(url)
来源：http://ugi.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yew.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://uek.shangyingyoupin.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zzj.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oxo.ivvv.top

[L02] 发送 POST JSON
来源：http://cpn.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zrz.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mmm.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tqc.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jds.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ibt.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qup.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://txr.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bny.yueranfly.top

[L03] 设置自定义请求头
来源：http://xts.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vcu.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ojk.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kno.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jas.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://orb.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uyo.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mhb.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wxs.wangdashe.top

[L04] 设置超时
来源：http://sjd.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://bwx.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ilg.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mbk.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://neq.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://acm.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ike.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bhc.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://czf.xinyue.icu

[L05] 上传文件（multipart）
来源：http://rjq.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cdd.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dlf.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ndo.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zxy.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cat.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zbw.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ryx.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cfn.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://oos.haohaochexian.top

Py:   resp.json()
来源：http://axz.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://api.birdmap.top

JS:   await resp.json()
来源：http://wgi.gogol.net.cn

TS:   await resp.json()
来源：http://pit.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxo.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yop.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://nae.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cel.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://jkb.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lcv.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fsx.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://qiv.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://tjr.jqgfzy.top

Java: resp.statusCode()
来源：http://acu.birdmap.top

Go:   resp.StatusCode
来源：http://ysz.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://kkl.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://utm.yuxming.cn

[L08] 并发请求多个地址
来源：http://dgt.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wnp.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://kho.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://emu.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hlq.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blj.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lyj.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mlf.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://liw.cucudq.cn

================================================================================
来源：http://xty.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://htj.yongpay.top

================================================================================
来源：http://oay.xylfe.cn

[M01] 读取命令行参数
来源：http://dtk.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://oeo.hcnkem.com

PHP:  $argv;  $argc;
来源：http://raw.redwolf501.top

JS:   process.argv.slice(2)
来源：http://als.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://tty.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://eku.gzhubu.top

Go:   os.Args[1:]
来源：http://dnm.hfpthk.cn

Ruby: ARGV
来源：http://zeq.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://lho.9152youxi.cn

[M02] 读取环境变量
来源：http://sge.bbcook.cn

Py:   os.environ.get("HOME")
来源：http://sgt.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pbj.sxryk.cn

JS:   process.env.HOME
来源：http://jrk.pengpengdd.cyou

TS:   process.env.HOME
来源：http://xjk.shuidangran.top

Java: System.getenv("HOME")
来源：http://zok.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cuu.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://axv.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rdb.xziqi.cn

[M03] 执行外部命令
来源：http://anj.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iuo.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zoi.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://asp.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://obb.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ixt.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://mgh.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://yjh.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://bbn.chenzaomai.com

[M04] 获取当前工作目录
来源：http://pvq.cheryme.top

Py:   os.getcwd()
来源：http://qgf.yvedp.cn

PHP:  getcwd();
来源：http://itl.sufxvd.cn

JS:   process.cwd()
来源：http://myz.ctjpmb.com

TS:   process.cwd()
来源：http://hyg.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://vou.jqgufenzy.top

Go:   os.Getwd()
来源：http://nnr.yj20258888.top

Ruby: Dir.pwd
来源：http://lzc.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://isj.sysykeji.top

[M05] 设置退出码
来源：http://kpw.ehwqpu.com

Py:   sys.exit(1)
来源：http://wcr.hammf.cn

PHP:  exit(1);
来源：http://kzb.andypj.xyz

JS:   process.exit(1)
来源：http://yvk.yj20258888.top

TS:   process.exit(1)
来源：http://ter.zhengqikj.top

Java: System.exit(1)
来源：http://ygn.guannengcc.top

Go:   os.Exit(1)
来源：http://tub.0kj1m.cn

Ruby: exit 1
来源：http://hgw.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hnu.tanke756.top

[M06] 向标准错误输出
来源：http://cvr.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://lih.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ghl.guowangkeji.top

JS:   console.error("err")
来源：http://tbt.cdnleiting.top

TS:   console.error("err")
来源：http://obf.hammf.cn

Java: System.err.println("err")
来源：http://ldr.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://exo.nwbrower.top

Ruby: warn "err"
来源：http://slc.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://xcs.hysaishi.cn

[M07] 判断是否为主入口
来源：http://sas.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://our.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qfk.vehdjk.com

JS:   require.main === module
来源：http://zrs.meibo888.top

TS:   require.main === module
来源：http://ctr.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://nuh.zdbjq.cn

Go:   func main()
来源：http://qne.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zdn.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://owf.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://djr.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://xuc.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://msm.haohaochexian.top

JS:   process.platform;  process.version
来源：http://ujp.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://glw.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sqf.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://fzv.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tpg.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://sol.hesvh.cn

================================================================================
来源：http://baq.xuanzx.com

N. 数据结构与算法
来源：http://dcq.gogol.net.cn

================================================================================
来源：http://qmb.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://xby.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mlq.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://thp.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wax.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dwq.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://mnf.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://wop.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://lhd.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sia.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://noh.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://ibp.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vre.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ato.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zln.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mgv.yonumen.top

Go:   slices.Sort(arr)
来源：http://jof.yj20258.top

Ruby: arr.sort
来源：http://gyj.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bze.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://qjw.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://stc.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://paq.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gry.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://czs.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oat.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pws.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yes.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://oym.0kj1m.cn

[N04] 斐波那契数列
来源：http://nzt.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zzj.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xpl.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dhh.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://waj.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqz.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nvp.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fbm.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tdc.chenjidiqi.icu

[N05] 最大公约数
来源：http://ybt.birdmap.top

Py:   math.gcd(a, b)
来源：http://kbx.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ikh.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cdy.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ent.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://btc.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qdo.9152youxi.cn

Ruby: a.gcd(b)
来源：http://ctl.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ocy.hnxiangtu.top

[N06] 判断回文字符串
来源：http://fsc.316326.xyz

Py:   s == s[::-1]
来源：http://cor.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://hhx.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://qzd.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://wbk.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ajs.epnwcf.com

Go:   // 双指针从两端比较
来源：http://mie.hfpthk.cn

Ruby: s == s.reverse
来源：http://tlo.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nlh.hammf.cn

[N07] 两数之和（返回下标）
来源：http://lbh.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fck.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://flw.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lbr.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://bai.jlsjyb.cn

Java: // 手写 HashMap
来源：http://xoh.havefunace.top

Go:   // 手写 map[int]int
来源：http://qop.316326.xyz

Ruby: // 手写 Hash
来源：http://cbv.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://tpo.hnxiangtu.top

[N08] 生成全排列
来源：http://qvl.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://vfb.sxryk.cn

PHP:  // 手写递归交换
来源：http://ffw.hesvh.cn

JS:   // 手写回溯递归
来源：http://umq.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://onf.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://bdi.havefunace.top

Go:   // 手写回溯递归
来源：http://xrq.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://twc.sysykeji.top

C#:   // 手写回溯递归
来源：http://ucz.smart0.xyz

[N09] 栈与队列
来源：http://fkd.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tri.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lwp.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iov.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qwa.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xug.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pfz.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wuj.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xxw.zhiwuduotai.top

[N10] 链表节点定义
来源：http://drj.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wov.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ziq.fehbvm.com


<!-- 参考信息 -->