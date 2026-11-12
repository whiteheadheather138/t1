代发 wailian999

[K02] JSON 字符串转对象
来源：http://ueu.svipenyu.cn

Py:   json.loads(s)
来源：http://gvy.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tzj.gotoacloud.top

JS:   JSON.parse(s)
来源：http://mny.smart0.xyz

TS:   JSON.parse(s)
来源：http://lcx.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jpa.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://ggk.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://ida.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://twv.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://cdq.sxryk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pfa.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bsy.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eny.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://keh.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oox.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://coy.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://oxq.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyl.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://iki.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bfr.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://owv.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aex.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zpu.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ewp.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qjp.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nac.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jhs.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://jqg.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://kwf.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://nxs.yvedp.cn

JS:   structuredClone(obj)
来源：http://vyh.yongpay.top

TS:   structuredClone(obj)
来源：http://tpm.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uek.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://izi.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://liy.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://wkl.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://vdn.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aaf.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oxv.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qvo.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vkm.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yke.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nae.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xjy.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ray.fengsongda.top

[K07] 进制转换
来源：http://ewo.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://juk.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cqa.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gea.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tux.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ftf.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gzd.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vny.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ypa.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://tqg.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://tlc.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pgu.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ojg.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://zdc.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pzk.cdnleiting.top

Go:   encoding/gob
来源：http://riq.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://xfr.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://plg.hnxiangtu.top

================================================================================
来源：http://mwh.shanyushiyangtech.top

L. 网络请求
来源：http://hhn.guannengcc.top

================================================================================
来源：http://ejm.yvedp.cn

[L01] 发送 GET 请求
来源：http://fcj.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nzv.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ttp.yuanzhike.top

JS:   await fetch(url)
来源：http://clm.cheryme.top

TS:   await fetch(url)
来源：http://wlt.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ffh.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://swl.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fyv.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xzt.haohaochexian.top

[L02] 发送 POST JSON
来源：http://epy.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://pag.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ttc.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usb.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lrq.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hls.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pxa.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ymk.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kxr.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://oki.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pqr.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qan.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ids.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eee.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fvu.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://idr.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://csx.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xsc.hywenlv.cn

[L04] 设置超时
来源：http://hbx.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://cmc.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nuy.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nqb.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewd.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://seq.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mlb.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cpk.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eok.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://bcf.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://imx.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mpm.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wgv.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zdp.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dct.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygu.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zkw.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cjl.meibo888.top

[L06] 解析响应为 JSON
来源：http://hgo.daxiang520.top

Py:   resp.json()
来源：http://cda.ydzc1.top

PHP:  json_decode($body, true);
来源：http://nwt.jqgfzy.top

JS:   await resp.json()
来源：http://lau.hnxiangtu.top

TS:   await resp.json()
来源：http://izx.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xcq.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iul.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://vbp.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ugr.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://fyc.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ury.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jji.cashguo.top

JS:   resp.ok;  resp.status
来源：http://ynv.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://bbe.jinqigufen.top

Java: resp.statusCode()
来源：http://olg.bjfxy.top

Go:   resp.StatusCode
来源：http://cek.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://zyo.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://jhi.epnwcf.com

[L08] 并发请求多个地址
来源：http://sgn.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wpw.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://wcs.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nua.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfv.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zrh.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vjw.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wjm.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ljq.cdnleiting.top

================================================================================
来源：http://tva.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://kxl.yuxming.cn

================================================================================
来源：http://zls.xziqi.cn

[M01] 读取命令行参数
来源：http://xkq.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://udr.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://klm.hcnkem.com

JS:   process.argv.slice(2)
来源：http://nnu.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://gwq.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://vln.gotoacloud.top

Go:   os.Args[1:]
来源：http://meo.zdqjudy.top

Ruby: ARGV
来源：http://okt.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://pqg.gzhubu.top

[M02] 读取环境变量
来源：http://jfw.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://xov.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ehc.andypj.xyz

JS:   process.env.HOME
来源：http://qqq.zycfv.cn

TS:   process.env.HOME
来源：http://ywi.jianghu66.top

Java: System.getenv("HOME")
来源：http://psz.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vah.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://fnk.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ijf.gogol.net.cn

[M03] 执行外部命令
来源：http://zdq.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qmu.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ftz.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://enb.bjfxy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xeu.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tls.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pqi.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lvf.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://dzi.zhengqikj.top

[M04] 获取当前工作目录
来源：http://gtg.xylfe.cn

Py:   os.getcwd()
来源：http://uis.fehbvm.com

PHP:  getcwd();
来源：http://uhp.vqdsnc.cn

JS:   process.cwd()
来源：http://xrh.yj20258888.top

TS:   process.cwd()
来源：http://qoi.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://bid.daria6918.cn

Go:   os.Getwd()
来源：http://mck.hysaishi.cn

Ruby: Dir.pwd
来源：http://lbb.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://fkr.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://hsi.xziqi.cn

Py:   sys.exit(1)
来源：http://baa.birdmap.top

PHP:  exit(1);
来源：http://dhg.tian-w.cn

JS:   process.exit(1)
来源：http://vap.zhixingplan.top

TS:   process.exit(1)
来源：http://jlp.uphjek.com

Java: System.exit(1)
来源：http://jkc.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://ica.andypj.xyz

Ruby: exit 1
来源：http://rqu.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gea.yvedp.cn

[M06] 向标准错误输出
来源：http://xge.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://iit.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pdw.cdnleiting.top

JS:   console.error("err")
来源：http://uxb.jinqigfzy.top

TS:   console.error("err")
来源：http://met.uphjek.com

Java: System.err.println("err")
来源：http://nwy.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nmh.birdmap.top

Ruby: warn "err"
来源：http://gpo.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://txi.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://oal.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://myr.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jup.vqdsnc.cn

JS:   require.main === module
来源：http://cxr.haohaochexian.top

TS:   require.main === module
来源：http://rah.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://dlw.redwolf501.top

Go:   func main()
来源：http://sje.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://inb.yj202588.top

C#:   static void Main(string[] args)
来源：http://yqd.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://mjm.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://tsu.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://nou.yongpay.top

JS:   process.platform;  process.version
来源：http://cbg.hysaishi.cn

TS:   process.platform;  process.version
来源：http://xjr.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kkv.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ydb.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tfk.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oyn.redwolf501.top

================================================================================
来源：http://sos.hnxiangtu.top

N. 数据结构与算法
来源：http://qcp.ydjk.org.cn

================================================================================
来源：http://ohe.cheryme.top

[N01] 二分查找（有序数组）
来源：http://jxj.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://hmz.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cwc.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrx.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cpx.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wmu.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://raw.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hcz.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://edk.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://ico.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://xzs.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qnt.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://flp.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://htj.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fqn.mhx1999.top

Go:   slices.Sort(arr)
来源：http://tmg.cashguo.top

Ruby: arr.sort
来源：http://yvp.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://scs.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://nau.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qmd.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://dph.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rmm.jiagoushi.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xfm.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://isn.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://axm.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kmx.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://ydl.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://sjg.ybcxt.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xpm.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://guz.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uzy.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vgf.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://shp.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vzk.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qlu.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbu.shanyushiyangtech.top

[N05] 最大公约数
来源：http://sjy.havefunace.top

Py:   math.gcd(a, b)
来源：http://bpb.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fko.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pvc.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tpn.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pwp.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vnl.epnwcf.com

Ruby: a.gcd(b)
来源：http://qjt.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fiq.ydzc1.top

[N06] 判断回文字符串
来源：http://stq.wangdashe.top

Py:   s == s[::-1]
来源：http://zfc.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://gyj.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://nwd.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://mvf.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kpp.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://mdk.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://hjw.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tlb.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://clq.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://znu.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ejj.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vck.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://fwi.zdbjq.cn

Java: // 手写 HashMap
来源：http://wbr.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://ebb.yuanzhike.top

Ruby: // 手写 Hash
来源：http://zhc.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ksk.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://sqg.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://wob.redwolf501.top

PHP:  // 手写递归交换
来源：http://zfz.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://rug.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://dyz.cdnleiting.top

Java: // 手写回溯递归
来源：http://wgu.bbcook.cn

Go:   // 手写回溯递归
来源：http://tlo.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://alk.cashguo.top

C#:   // 手写回溯递归
来源：http://mqm.9152youxi.cn

[N09] 栈与队列
来源：http://hsr.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hem.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ahj.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gnp.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dsu.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lxd.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dbq.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://umj.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iyh.dianchejie.cn

[N10] 链表节点定义
来源：http://zpw.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vpb.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eus.zdbjq.cn


<!-- 参考信息 -->