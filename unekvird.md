代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qcw.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nvl.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://nwt.cheryme.top

TS:   JSON.stringify(obj)
来源：http://qzk.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://avd.epnwcf.com

Go:   json.Marshal(obj)
来源：http://lhx.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zjh.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vom.daxiang520.top

[K02] JSON 字符串转对象
来源：http://wmo.fehbvm.com

Py:   json.loads(s)
来源：http://wrt.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://koq.dianchejie.cn

JS:   JSON.parse(s)
来源：http://bko.hnqzz.top

TS:   JSON.parse(s)
来源：http://aph.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://taf.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://vol.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://fiv.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cwd.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://whx.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lov.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rla.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gek.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://eqk.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bqv.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hnf.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rce.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oej.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://yyg.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cbj.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sto.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yrm.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kmi.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mzu.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wdd.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tkd.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wvd.zhoulong.xyz

[K05] 深拷贝对象
来源：http://avt.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://gpx.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://oiz.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://jyo.guannengcc.top

TS:   structuredClone(obj)
来源：http://baq.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ble.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://olp.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uod.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://djt.pycfn.com

[K06] 解析 URL 查询串
来源：http://pfq.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://alr.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iqa.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cqu.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bzh.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ryq.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kgm.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://roa.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tco.cheryme.top

[K07] 进制转换
来源：http://mad.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kqh.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ejn.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tbp.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://piw.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vil.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ber.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ole.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cqt.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://mph.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://jiz.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://orv.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://ims.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://yrw.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eip.sysykeji.top

Go:   encoding/gob
来源：http://ohq.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://rac.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zwp.cheryme.top

================================================================================
来源：http://hkd.cqqwz.cn

L. 网络请求
来源：http://qar.ehwqpu.com

================================================================================
来源：http://dox.pycfn.com

[L01] 发送 GET 请求
来源：http://zlb.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qbd.pengpengdd.cyou

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ncc.hfpthk.cn

JS:   await fetch(url)
来源：http://lvy.yueranfly.top

TS:   await fetch(url)
来源：http://nds.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://owj.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://xia.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yxz.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kxd.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://lvt.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://glg.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hxj.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zex.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sze.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://spx.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rxb.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ank.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fji.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://wuh.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ggc.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cqo.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aoc.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebs.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mhv.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wxm.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://chd.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jnq.ydjk.org.cn

[L04] 设置超时
来源：http://erv.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://pwi.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ihs.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewj.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eyj.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://faz.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hag.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wtk.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lck.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://wbd.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://glh.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oiy.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://omh.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://srn.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sro.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xxm.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qbn.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eao.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://jol.sweek.top

Py:   resp.json()
来源：http://moo.cucudq.cn

PHP:  json_decode($body, true);
来源：http://mrb.yj20258888.top

JS:   await resp.json()
来源：http://qef.vehdjk.com

TS:   await resp.json()
来源：http://oep.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vzl.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uaw.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://adr.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bzs.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://buk.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cby.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lxe.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://lwy.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://rfv.yangfankeji.com

Java: resp.statusCode()
来源：http://vke.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://ulx.xylfe.cn

Ruby: resp.code.to_i
来源：http://fsw.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://uve.zycfv.cn

[L08] 并发请求多个地址
来源：http://pum.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fbo.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://yup.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dkl.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dal.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nwr.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fad.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prv.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rdc.cdnleiting.top

================================================================================
来源：http://fvk.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://xdl.yvedp.cn

================================================================================
来源：http://eyc.0kj1m.cn

[M01] 读取命令行参数
来源：http://jsw.shuidangran.top

Py:   sys.argv[1:]
来源：http://zyu.yfazqb.com

PHP:  $argv;  $argc;
来源：http://xrg.52xcode.cn

JS:   process.argv.slice(2)
来源：http://yam.yfazqb.com

TS:   process.argv.slice(2)
来源：http://wuj.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://smm.bjfxy.top

Go:   os.Args[1:]
来源：http://aqm.aibaodan.cn

Ruby: ARGV
来源：http://jeu.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://wjt.havefunace.top

[M02] 读取环境变量
来源：http://xhm.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://uaq.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://atq.kuanghao11.cn

JS:   process.env.HOME
来源：http://zgf.sxryk.cn

TS:   process.env.HOME
来源：http://gyf.meibo888.top

Java: System.getenv("HOME")
来源：http://lde.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://poy.yj202588.top

Ruby: ENV["HOME"]
来源：http://via.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wrj.aibaodan.cn

[M03] 执行外部命令
来源：http://wqe.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wlw.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wqu.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ihn.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uop.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gyu.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wxg.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vks.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://vjt.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://fum.yonumen.top

Py:   os.getcwd()
来源：http://ahe.nwbrower.top

PHP:  getcwd();
来源：http://oth.snrcjt.cn

JS:   process.cwd()
来源：http://ssx.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://dea.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://kwu.sjlbkw.cn

Go:   os.Getwd()
来源：http://ehn.cdnleiting.top

Ruby: Dir.pwd
来源：http://mcg.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://gfy.zhengqikj.top

[M05] 设置退出码
来源：http://wnr.hywenlv.cn

Py:   sys.exit(1)
来源：http://cht.vehdjk.com

PHP:  exit(1);
来源：http://lpk.zhengqikj.top

JS:   process.exit(1)
来源：http://kyd.hysaishi.cn

TS:   process.exit(1)
来源：http://zxz.jinqigfzy.top

Java: System.exit(1)
来源：http://eww.shzxlz.cn

Go:   os.Exit(1)
来源：http://wnv.redwolf501.top

Ruby: exit 1
来源：http://cmp.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ihm.yueranfly.top

[M06] 向标准错误输出
来源：http://eji.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://sbe.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://pbe.quarkkingdee.top

JS:   console.error("err")
来源：http://ryz.yj20258888.top

TS:   console.error("err")
来源：http://mvu.shuidangran.top

Java: System.err.println("err")
来源：http://uad.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mps.zdqjudy.top

Ruby: warn "err"
来源：http://abs.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://mas.yvedp.cn

[M07] 判断是否为主入口
来源：http://xzc.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://fyz.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ndp.hongshengwenyu.top

JS:   require.main === module
来源：http://uzv.yonumen.top

TS:   require.main === module
来源：http://bhe.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://vwx.hnxiangtu.top

Go:   func main()
来源：http://jxq.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qne.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://pzv.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://ghc.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://hqx.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://enu.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://xzp.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://lke.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gix.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vlv.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nga.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jnt.zhoulong.xyz

================================================================================
来源：http://yun.ybcxt.top

N. 数据结构与算法
来源：http://bcz.ywan-chungtsiang.top

================================================================================
来源：http://cnv.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://phh.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vvm.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hwr.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qer.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ugb.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://yjl.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ddk.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zzd.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://nhu.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://hxm.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://hjp.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hye.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://kjn.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qdc.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ydh.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://lgb.gogol.net.cn

Ruby: arr.sort
来源：http://ris.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://guz.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://mxt.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wzm.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://xzb.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ryb.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvg.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hzu.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dut.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lra.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://zfu.redwolf501.top

[N04] 斐波那契数列
来源：http://ize.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qdt.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://phw.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhh.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nzu.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://prq.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cdd.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://klq.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hzl.yj20258.top

[N05] 最大公约数
来源：http://hms.mhx1999.top

Py:   math.gcd(a, b)
来源：http://lsf.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ssj.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dgh.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixp.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mmp.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fxy.bbcook.cn

Ruby: a.gcd(b)
来源：http://afv.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kgf.hcnkem.com

[N06] 判断回文字符串
来源：http://llw.jlsjyb.cn

Py:   s == s[::-1]
来源：http://xio.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://rga.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://ptt.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://qcp.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zwh.yj202588.top

Go:   // 双指针从两端比较
来源：http://ybn.zdbjq.cn

Ruby: s == s.reverse
来源：http://ygn.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ztp.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://dkc.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dxs.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wod.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qst.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://jij.hcnkem.com

Java: // 手写 HashMap
来源：http://cns.xylfe.cn

Go:   // 手写 map[int]int
来源：http://vru.yangfankeji.com

Ruby: // 手写 Hash
来源：http://fkx.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://jyf.jiagoushi.top

[N08] 生成全排列
来源：http://ofa.uphjek.com

Py:   itertools.permutations(arr)
来源：http://hve.yj202588.top

PHP:  // 手写递归交换
来源：http://tpt.birdmap.top

JS:   // 手写回溯递归
来源：http://rlm.meibo888.top

TS:   // 手写回溯递归
来源：http://zrc.pycfn.com

Java: // 手写回溯递归
来源：http://xrm.daria6918.cn

Go:   // 手写回溯递归
来源：http://izm.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://iqr.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://wxy.fanxiaobao.xyz

[N09] 栈与队列
来源：http://nio.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ooa.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ohe.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jbe.yj202588.top


<!-- 参考信息 -->