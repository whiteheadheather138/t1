代发 wailian999

[K02] JSON 字符串转对象
来源：http://ufe.jlsjyb.cn

Py:   json.loads(s)
来源：http://hjl.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://afn.xylfe.cn

JS:   JSON.parse(s)
来源：http://oxf.ctjpmb.com

TS:   JSON.parse(s)
来源：http://juk.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dhg.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://yos.meibo888.top

Ruby: JSON.parse(s)
来源：http://bjy.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kpk.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://pwv.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gvs.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uxb.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ioi.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gxj.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bev.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://guo.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fwj.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xzw.fktsv.cn

[K04] 读取 JSON 文件
来源：http://qam.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://alp.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://asq.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xbp.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfc.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vgr.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rcf.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://jhe.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sjq.zhongyouzk.top

[K05] 深拷贝对象
来源：http://bbo.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://ktr.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://yyt.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://rbg.yvedp.cn

TS:   structuredClone(obj)
来源：http://xuk.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uhs.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fqb.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jkb.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uco.fzhhl.top

[K06] 解析 URL 查询串
来源：http://wum.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kuc.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gqe.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://psx.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lzu.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ucy.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tzd.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aqe.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vid.316326.xyz

[K07] 进制转换
来源：http://kpe.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aaz.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zoo.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://veq.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kpz.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ggf.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://was.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://efj.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xdg.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://sbv.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://kzm.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://khz.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://axm.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://ndv.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qfz.yvedp.cn

Go:   encoding/gob
来源：http://aux.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://kwd.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vmf.gogol.net.cn

================================================================================
来源：http://uqs.svipenyu.cn

L. 网络请求
来源：http://kwt.bbcook.cn

================================================================================
来源：http://yjo.tian-w.cn

[L01] 发送 GET 请求
来源：http://yns.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vrr.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://chj.c1oappe.top

JS:   await fetch(url)
来源：http://wbx.cheryme.top

TS:   await fetch(url)
来源：http://qjr.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gnu.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://xbp.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nml.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://njw.sweek.top

[L02] 发送 POST JSON
来源：http://dry.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rdw.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sar.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljy.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xnn.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lwq.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zgz.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xkh.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eqw.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://gqj.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qkk.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zny.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbd.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbk.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xkp.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lxa.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qes.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xwx.ppjwa.cn

[L04] 设置超时
来源：http://usx.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://vff.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://isz.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nnr.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ppy.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wvp.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://brz.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kdo.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://git.vehdjk.com

[L05] 上传文件（multipart）
来源：http://ypt.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kfk.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xxx.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kzg.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oii.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zbb.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iqd.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://izs.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qri.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://ikj.xuetiantiany.cn

Py:   resp.json()
来源：http://rsm.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://ins.daxiang520.top

JS:   await resp.json()
来源：http://wls.zhengqikj.top

TS:   await resp.json()
来源：http://bbw.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lbh.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://krz.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://mzn.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fnk.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://fvp.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dgz.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lfg.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://cuo.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://tpm.zhongyouzk.top

Java: resp.statusCode()
来源：http://kic.yongpay.top

Go:   resp.StatusCode
来源：http://vgw.xylfe.cn

Ruby: resp.code.to_i
来源：http://pot.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://wmz.yj20258.top

[L08] 并发请求多个地址
来源：http://wws.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mrq.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://nvr.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://not.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uzl.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oyb.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xni.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jxd.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cwd.cashguo.top

================================================================================
来源：http://idp.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://gud.ppjwa.cn

================================================================================
来源：http://fjb.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://dae.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://gvp.tarul.cn

PHP:  $argv;  $argc;
来源：http://mfh.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://yiu.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://kht.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://klx.guowangkeji.top

Go:   os.Args[1:]
来源：http://ghi.jqgufenzy.top

Ruby: ARGV
来源：http://otk.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://gci.guowangkeji.top

[M02] 读取环境变量
来源：http://iee.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://czi.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ujh.andypj.xyz

JS:   process.env.HOME
来源：http://lhr.dashuyun.cn

TS:   process.env.HOME
来源：http://kev.cucudq.cn

Java: System.getenv("HOME")
来源：http://mnk.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mcf.cashguo.top

Ruby: ENV["HOME"]
来源：http://uvu.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hep.kuanghao11.cn

[M03] 执行外部命令
来源：http://djm.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hif.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gjt.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://bmf.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://fmt.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hgk.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://htm.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://uox.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://rer.yj20258888.top

[M04] 获取当前工作目录
来源：http://vyp.yj20258888.top

Py:   os.getcwd()
来源：http://zao.yfazqb.com

PHP:  getcwd();
来源：http://lrc.yongpay.top

JS:   process.cwd()
来源：http://tug.yj20258888.top

TS:   process.cwd()
来源：http://qzb.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://qqf.ctjpmb.com

Go:   os.Getwd()
来源：http://glr.jiagoushi.top

Ruby: Dir.pwd
来源：http://ysi.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://jdb.guowangkeji.top

[M05] 设置退出码
来源：http://ghp.nanxinkj.top

Py:   sys.exit(1)
来源：http://qhq.epnwcf.com

PHP:  exit(1);
来源：http://cfo.c1oappe.top

JS:   process.exit(1)
来源：http://lat.wangshuangyany.cn

TS:   process.exit(1)
来源：http://wjm.jyoumei.cn

Java: System.exit(1)
来源：http://rqi.nanxinkj.top

Go:   os.Exit(1)
来源：http://nlz.mhx1999.top

Ruby: exit 1
来源：http://omm.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://odq.yongpay.top

[M06] 向标准错误输出
来源：http://jyi.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://dfm.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vzm.quarkkingdee.top

JS:   console.error("err")
来源：http://iwn.yongpay.top

TS:   console.error("err")
来源：http://qpo.ybcxt.top

Java: System.err.println("err")
来源：http://ivt.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dvq.jiagoushi.top

Ruby: warn "err"
来源：http://jay.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://spe.shuidangran.top

[M07] 判断是否为主入口
来源：http://dhx.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://sct.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pry.wangdashe.top

JS:   require.main === module
来源：http://cnz.zhengqikj.top

TS:   require.main === module
来源：http://vlu.cashguo.top

Java: public static void main(String[] args)
来源：http://kan.gotoacloud.top

Go:   func main()
来源：http://awf.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://evm.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://okw.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://wvc.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://mgf.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://gdl.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://mjc.xuanzx.com

TS:   process.platform;  process.version
来源：http://jkk.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xkj.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://edc.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tdx.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ugi.daria6918.cn

================================================================================
来源：http://ukc.yangfankeji.com

N. 数据结构与算法
来源：http://mpv.sufxvd.cn

================================================================================
来源：http://pno.uphjek.com

[N01] 二分查找（有序数组）
来源：http://rxk.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://sed.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ynu.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fvh.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dsy.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://xfv.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://xwi.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zua.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://ary.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://tyq.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://awg.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mvu.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dtx.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tly.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://knk.52xcode.cn

Go:   slices.Sort(arr)
来源：http://gar.ybcxt.top

Ruby: arr.sort
来源：http://zcd.jinqigfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yvl.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://pab.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xxt.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://xwb.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mzt.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sld.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hem.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lvm.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fvd.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fek.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://qnw.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ouy.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dyb.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://alh.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sdy.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pqs.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bsz.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ipe.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://etu.jqgufenzy.top

[N05] 最大公约数
来源：http://ewk.hnqzz.top

Py:   math.gcd(a, b)
来源：http://ncr.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://arh.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fzd.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ucp.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kvu.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wbm.52xcode.cn

Ruby: a.gcd(b)
来源：http://otd.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mqy.ydzc1.top

[N06] 判断回文字符串
来源：http://yoy.andypj.xyz

Py:   s == s[::-1]
来源：http://bhi.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://ncm.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://joy.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://zru.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jbw.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://azj.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://dmz.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qrp.hammf.cn

[N07] 两数之和（返回下标）
来源：http://iay.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://szw.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ztv.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fog.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://ggh.yuxming.cn

Java: // 手写 HashMap
来源：http://jbx.aibaodan.cn

Go:   // 手写 map[int]int
来源：http://xpn.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://hny.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cya.hnxiangtu.top

[N08] 生成全排列
来源：http://lsp.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://ahy.fehbvm.com

PHP:  // 手写递归交换
来源：http://wmc.shuidangran.top

JS:   // 手写回溯递归
来源：http://kvq.gzhubu.top

TS:   // 手写回溯递归
来源：http://nax.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://all.wangdashe.top

Go:   // 手写回溯递归
来源：http://mel.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://qdw.meibo888.top

C#:   // 手写回溯递归
来源：http://mwk.yj20258888.top

[N09] 栈与队列
来源：http://oik.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dbg.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lbz.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://whr.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uhp.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://twq.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rjj.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fxy.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ukk.zhoulong.xyz

[N10] 链表节点定义
来源：http://qqn.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ugs.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uxm.jqgufenzy.top


<!-- 参考信息 -->