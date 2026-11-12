代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ime.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://uhe.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://hld.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xzt.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://jlc.daxiang520.top

Py:   json.loads(s)
来源：http://xtv.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bbe.hnqzz.top

JS:   JSON.parse(s)
来源：http://qiy.pycfn.com

TS:   JSON.parse(s)
来源：http://mag.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mof.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://dxt.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://wpw.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qce.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://ieb.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bmj.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mty.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aat.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://czz.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hub.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ruv.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cxk.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fwt.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://yrz.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eys.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gfp.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iou.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wke.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tsw.guowangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pkc.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://xes.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nvc.52xcode.cn

[K05] 深拷贝对象
来源：http://aeq.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://knp.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://ckl.xinyue.icu

JS:   structuredClone(obj)
来源：http://jvz.hcnkem.com

TS:   structuredClone(obj)
来源：http://qzg.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vwz.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jau.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lkd.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://afz.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://oqw.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hkv.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qcw.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ype.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yql.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://apv.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://avv.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rek.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nyb.jyoumei.cn

[K07] 进制转换
来源：http://rnb.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sjh.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://upa.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://adc.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oge.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://snj.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ult.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fdj.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pzf.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://glz.yuxming.cn

Py:   pickle.dumps(obj)
来源：http://qux.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iwr.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://opc.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://kif.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://czd.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://yhr.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://hex.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tic.epnwcf.com

================================================================================
来源：http://bqm.zycfv.cn

L. 网络请求
来源：http://zcn.pycfn.com

================================================================================
来源：http://sei.yueranfly.top

[L01] 发送 GET 请求
来源：http://igq.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rqw.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zjg.0kj1m.cn

JS:   await fetch(url)
来源：http://trd.uphjek.com

TS:   await fetch(url)
来源：http://aqi.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ozb.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://fdf.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hfy.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hss.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://nir.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ard.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ppc.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kwr.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eva.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://toa.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://apj.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://afd.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rtf.hysaishi.cn

[L03] 设置自定义请求头
来源：http://yph.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fft.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bhg.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fqj.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ddn.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tdr.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aab.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rtv.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lqj.zhijiandao.cn

[L04] 设置超时
来源：http://dcw.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://isx.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ymr.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ngb.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wgh.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bwg.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nfw.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://suq.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://myx.c1oappe.top

[L05] 上传文件（multipart）
来源：http://jdk.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://prf.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xdc.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://txr.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sxw.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zey.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oad.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yiu.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://udr.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://hme.vqdsnc.cn

Py:   resp.json()
来源：http://dul.yfazqb.com

PHP:  json_decode($body, true);
来源：http://tws.fehbvm.com

JS:   await resp.json()
来源：http://wgj.hongshengwenyu.top

TS:   await resp.json()
来源：http://zeh.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uvw.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lds.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://qot.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xzy.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://bfk.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bzo.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xtw.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://akj.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://vvs.jianghu66.top

Java: resp.statusCode()
来源：http://wrw.yangfankeji.com

Go:   resp.StatusCode
来源：http://tye.cheryme.top

Ruby: resp.code.to_i
来源：http://rje.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://mgw.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://vaw.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kxk.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://jaw.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eig.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vop.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hqh.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vnj.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qfd.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ozi.yanxiufei.cn

================================================================================
来源：http://vcd.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://qso.vqdsnc.cn

================================================================================
来源：http://tqu.gaohongyu789.top

[M01] 读取命令行参数
来源：http://dfh.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://dfw.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://ort.shuidangran.top

JS:   process.argv.slice(2)
来源：http://tcq.ivvv.top

TS:   process.argv.slice(2)
来源：http://odc.cheryme.top

Java: args 数组（main 方法参数）
来源：http://oht.kuanghao11.cn

Go:   os.Args[1:]
来源：http://xow.jinyuanbaomall.cn

Ruby: ARGV
来源：http://num.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://xrz.wangdashe.top

[M02] 读取环境变量
来源：http://rvm.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://ccb.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://msn.zhijiandao.cn

JS:   process.env.HOME
来源：http://jbk.shuidangran.top

TS:   process.env.HOME
来源：http://ojw.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://tim.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fnl.fengsongda.top

Ruby: ENV["HOME"]
来源：http://ext.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ixg.cashguo.top

[M03] 执行外部命令
来源：http://dnm.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jtj.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ips.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gvu.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fkq.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gdr.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jjg.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://duw.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://vlx.svipenyu.cn

[M04] 获取当前工作目录
来源：http://nrb.cheryme.top

Py:   os.getcwd()
来源：http://vgf.ivvv.top

PHP:  getcwd();
来源：http://rqn.zhoulong.xyz

JS:   process.cwd()
来源：http://itk.redwolf501.top

TS:   process.cwd()
来源：http://vhs.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://zoa.hywenlv.cn

Go:   os.Getwd()
来源：http://bui.tian-w.cn

Ruby: Dir.pwd
来源：http://ohu.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://gst.zhoulong.xyz

[M05] 设置退出码
来源：http://qyp.9152youxi.cn

Py:   sys.exit(1)
来源：http://ket.sufxvd.cn

PHP:  exit(1);
来源：http://loa.shzxlz.cn

JS:   process.exit(1)
来源：http://yok.xylfe.cn

TS:   process.exit(1)
来源：http://ofr.yueranfly.top

Java: System.exit(1)
来源：http://leb.shuidangran.top

Go:   os.Exit(1)
来源：http://mec.bbcook.cn

Ruby: exit 1
来源：http://ibg.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gjl.ppjwa.cn

[M06] 向标准错误输出
来源：http://pdk.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://imh.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tcg.ppjwa.cn

JS:   console.error("err")
来源：http://knk.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://ddj.yueranfly.top

Java: System.err.println("err")
来源：http://cru.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://raq.wangdashe.top

Ruby: warn "err"
来源：http://hce.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://bpt.hammf.cn

[M07] 判断是否为主入口
来源：http://qmp.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://atr.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vuo.cqqwz.cn

JS:   require.main === module
来源：http://euu.meibo888.top

TS:   require.main === module
来源：http://kmj.yj20258.top

Java: public static void main(String[] args)
来源：http://eok.shzxlz.cn

Go:   func main()
来源：http://esy.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lkk.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://ipu.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://dne.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://qpd.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://edx.yueranfly.top

JS:   process.platform;  process.version
来源：http://twx.hnqzz.top

TS:   process.platform;  process.version
来源：http://yss.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bik.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ysu.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dju.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://weo.daxiang520.top

================================================================================
来源：http://rya.daria6918.cn

N. 数据结构与算法
来源：http://evq.yangfankeji.com

================================================================================
来源：http://ymx.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://mja.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://dyo.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ztk.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rrk.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hox.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://cbw.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://kxk.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wad.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://peg.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://tmm.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://boz.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ujh.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lsi.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tow.xuanzx.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uqh.yj202588.top

Go:   slices.Sort(arr)
来源：http://lwm.tian-w.cn

Ruby: arr.sort
来源：http://xsy.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zee.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://nxz.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fjb.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://ajh.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zmx.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mqg.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uek.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qiu.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qpb.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://tui.tian-w.cn

[N04] 斐波那契数列
来源：http://evp.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bbl.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yto.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://evq.andypj.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aoz.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vva.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oly.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://etg.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dik.dashuyun.cn

[N05] 最大公约数
来源：http://mhb.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://mfr.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://scs.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dtd.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fin.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xzp.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pap.dianchejie.cn

Ruby: a.gcd(b)
来源：http://lad.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oco.tian-w.cn

[N06] 判断回文字符串
来源：http://glj.yj20258.top

Py:   s == s[::-1]
来源：http://htm.xziqi.cn

PHP:  $s === strrev($s);
来源：http://fpg.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://zud.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://klk.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pmh.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://hly.mhx1999.top

Ruby: s == s.reverse
来源：http://ngf.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://wpa.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://ihc.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zhi.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cqd.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://zau.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://feu.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://hnb.yj202588.top

Go:   // 手写 map[int]int
来源：http://sal.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://rhe.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lgu.ydjk.org.cn

[N08] 生成全排列
来源：http://lqo.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://zgp.316326.xyz

PHP:  // 手写递归交换
来源：http://dcc.sxryk.cn

JS:   // 手写回溯递归
来源：http://ydm.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://dtm.svipenyu.cn

Java: // 手写回溯递归
来源：http://fqi.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://cac.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://mol.cdnleiting.top

C#:   // 手写回溯递归
来源：http://dva.jlsjyb.cn

[N09] 栈与队列
来源：http://spw.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hzu.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zkb.cdnleiting.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hyq.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qqz.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://owe.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hwn.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wwe.jinyuanbaomall.cn


<!-- 参考信息 -->