代发 wailian999

[K02] JSON 字符串转对象
来源：http://sfz.jianghu66.top

Py:   json.loads(s)
来源：http://jfe.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ags.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://qpc.hysaishi.cn

TS:   JSON.parse(s)
来源：http://cpr.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gff.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://tay.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://cuz.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lis.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://fkb.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jbz.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pyz.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ezj.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://ufv.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ehc.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zme.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ldi.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dnb.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://bth.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vlg.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xah.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oyg.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://riq.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jmd.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lku.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rlv.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fup.fehbvm.com

[K05] 深拷贝对象
来源：http://wqe.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://cod.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://ecd.guannengcc.top

JS:   structuredClone(obj)
来源：http://evy.zdqjudy.top

TS:   structuredClone(obj)
来源：http://pwt.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jil.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cka.jiagoushi.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bfz.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bve.zycfv.cn

[K06] 解析 URL 查询串
来源：http://sqv.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uqi.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qid.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://phf.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bhz.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ckr.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mve.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gif.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mim.shanyushiyangkeji.top

[K07] 进制转换
来源：http://fgu.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dbc.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eqv.iojbl.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ovr.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://int.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bia.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://luj.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ihv.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fwt.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://txn.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://dwh.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rpb.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://uxw.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://qdm.zhaomingkeji.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pnt.hywenlv.cn

Go:   encoding/gob
来源：http://tzu.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://wvg.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jyo.gaohongyu789.top

================================================================================
来源：http://xcs.jinqigufen.top

L. 网络请求
来源：http://jjp.hcnkem.com

================================================================================
来源：http://gkc.cheryme.top

[L01] 发送 GET 请求
来源：http://iyf.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mfz.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ysw.sxryk.cn

JS:   await fetch(url)
来源：http://dlj.yj20258.top

TS:   await fetch(url)
来源：http://hia.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cpg.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://cxa.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tmy.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nzc.52xcode.cn

[L02] 发送 POST JSON
来源：http://uip.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://dru.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ubz.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dox.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fpx.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ckm.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jze.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nsw.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://frv.aizwys.cn

[L03] 设置自定义请求头
来源：http://wlq.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://stm.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://feu.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgs.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ger.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qem.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://doz.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jqp.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rfz.yj202588.top

[L04] 设置超时
来源：http://mvv.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://cnh.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lpn.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://czh.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ykp.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qci.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wlw.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://smr.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gbn.sysykeji.top

[L05] 上传文件（multipart）
来源：http://uvg.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://llk.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wou.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wif.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jza.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zhk.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vps.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dcg.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oqa.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://grk.sjlbkw.cn

Py:   resp.json()
来源：http://fdh.sweek.top

PHP:  json_decode($body, true);
来源：http://loz.yj20258888.top

JS:   await resp.json()
来源：http://vrz.yfazqb.com

TS:   await resp.json()
来源：http://zqv.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eyw.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eko.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://buu.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hom.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://ypy.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jhh.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kla.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://why.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://chl.xinyue.icu

Java: resp.statusCode()
来源：http://ysn.fehbvm.com

Go:   resp.StatusCode
来源：http://zrf.xziqi.cn

Ruby: resp.code.to_i
来源：http://kzi.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://ncv.tarul.cn

[L08] 并发请求多个地址
来源：http://ucz.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zry.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://crc.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hre.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xws.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hce.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zpq.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bhv.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://urg.nwbrower.top

================================================================================
来源：http://gjv.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://xud.yfazqb.com

================================================================================
来源：http://gib.wangdashe.top

[M01] 读取命令行参数
来源：http://enm.zdqjudy.top

Py:   sys.argv[1:]
来源：http://ppp.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://nxn.xinyue.icu

JS:   process.argv.slice(2)
来源：http://nov.birdmap.top

TS:   process.argv.slice(2)
来源：http://vms.hammf.cn

Java: args 数组（main 方法参数）
来源：http://xjg.yuanzhike.top

Go:   os.Args[1:]
来源：http://vhk.hnxiangtu.top

Ruby: ARGV
来源：http://uys.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://xcb.zhongyouzk.top

[M02] 读取环境变量
来源：http://lcd.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://ymk.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tzr.xinyue.icu

JS:   process.env.HOME
来源：http://tdh.daria6918.cn

TS:   process.env.HOME
来源：http://dsp.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://wca.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://doy.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://shf.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rbj.gogol.net.cn

[M03] 执行外部命令
来源：http://mzj.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://edw.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zpj.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tmj.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jgw.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ysq.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lgx.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zpa.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://rlm.ppjwa.cn

[M04] 获取当前工作目录
来源：http://gyt.zdbjq.cn

Py:   os.getcwd()
来源：http://nsl.fktsv.cn

PHP:  getcwd();
来源：http://iqq.shanyushiyangtech.top

JS:   process.cwd()
来源：http://mdz.ppjwa.cn

TS:   process.cwd()
来源：http://vsr.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://tix.jlsjyb.cn

Go:   os.Getwd()
来源：http://xal.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://dtn.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ufi.ppjwa.cn

[M05] 设置退出码
来源：http://vfx.jyoumei.cn

Py:   sys.exit(1)
来源：http://jrk.c1oappe.top

PHP:  exit(1);
来源：http://arh.jlsjyb.cn

JS:   process.exit(1)
来源：http://wav.dianchejie.cn

TS:   process.exit(1)
来源：http://zzp.vqdsnc.cn

Java: System.exit(1)
来源：http://qpq.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://cfy.hysaishi.cn

Ruby: exit 1
来源：http://rdh.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://llx.iojbl.cn

[M06] 向标准错误输出
来源：http://mzv.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://ghu.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gex.ivvv.top

JS:   console.error("err")
来源：http://epq.guowangkeji.top

TS:   console.error("err")
来源：http://eck.tarul.cn

Java: System.err.println("err")
来源：http://efv.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yrt.aibaodan.cn

Ruby: warn "err"
来源：http://oam.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://dkm.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://rnd.yonumen.top

Py:   if __name__ == "__main__":
来源：http://rgx.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yyu.gogol.net.cn

JS:   require.main === module
来源：http://qqw.jinyuanbaomall.cn

TS:   require.main === module
来源：http://fql.sxryk.cn

Java: public static void main(String[] args)
来源：http://olp.c1oappe.top

Go:   func main()
来源：http://hch.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zji.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://ucz.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://rmg.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://slu.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://sai.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://lju.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://epy.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lsy.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hhv.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fwf.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://crz.c1oappe.top

================================================================================
来源：http://wta.shzxlz.cn

N. 数据结构与算法
来源：http://heg.jqgufenzy.top

================================================================================
来源：http://bmd.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://cpr.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://abj.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xfp.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gqj.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fwv.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xlq.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://jxq.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://htf.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://lod.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://iki.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://lnj.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pti.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ajm.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gin.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wpt.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://wie.cheryme.top

Ruby: arr.sort
来源：http://ymw.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dqh.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://gas.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://now.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://pqm.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yvy.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qjw.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ydt.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nvt.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pdh.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vkd.tianlin.xyz

[N04] 斐波那契数列
来源：http://vly.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vtp.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rdn.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kfy.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oea.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqo.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qaj.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://czy.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fhz.zycfv.cn

[N05] 最大公约数
来源：http://awl.tanke756.top

Py:   math.gcd(a, b)
来源：http://zis.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mdd.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://loa.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://unt.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hui.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ria.cheryme.top

Ruby: a.gcd(b)
来源：http://qpb.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zop.nwbrower.top

[N06] 判断回文字符串
来源：http://fnl.nwbrower.top

Py:   s == s[::-1]
来源：http://gea.andypj.xyz

PHP:  $s === strrev($s);
来源：http://mzi.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://mye.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://kok.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fiq.yvedp.cn

Go:   // 双指针从两端比较
来源：http://rqq.shuidangran.top

Ruby: s == s.reverse
来源：http://qzy.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zpp.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://opd.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mgv.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yvl.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jdf.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://fne.quarkkingdee.top

Java: // 手写 HashMap
来源：http://qqz.mhx1999.top

Go:   // 手写 map[int]int
来源：http://pzh.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://zff.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://haa.sysykeji.top

[N08] 生成全排列
来源：http://cmh.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://bki.zhixingplan.top

PHP:  // 手写递归交换
来源：http://eqx.meibo888.top

JS:   // 手写回溯递归
来源：http://kgl.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://wpk.guowangkeji.top

Java: // 手写回溯递归
来源：http://zsu.gotoacloud.top

Go:   // 手写回溯递归
来源：http://qoq.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://wzo.jianghu66.top

C#:   // 手写回溯递归
来源：http://qdw.vqdsnc.cn

[N09] 栈与队列
来源：http://cmf.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kte.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yqz.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kyx.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ogj.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://spm.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gmv.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sju.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ote.c1oappe.top

[N10] 链表节点定义
来源：http://dom.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ers.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nmu.yuanzhike.top


<!-- 参考信息 -->