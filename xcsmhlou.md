代发 wailian999

================================================================================
来源：http://qpo.aizwys.cn

K. JSON 与序列化
来源：http://qme.hnxiangtu.top

================================================================================
来源：http://gpn.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://xex.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kto.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jrf.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://oav.meibo888.top

TS:   JSON.stringify(obj)
来源：http://fvu.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ehw.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://bsr.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://ksj.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lxh.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://ewf.gotoacloud.top

Py:   json.loads(s)
来源：http://sxm.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zsa.shuidangran.top

JS:   JSON.parse(s)
来源：http://yjx.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://hup.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ddd.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://pkb.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://jpk.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bxl.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://ege.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://grn.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tyq.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://prd.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vxp.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fzz.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ege.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://puk.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aln.daxiang520.top

[K04] 读取 JSON 文件
来源：http://bon.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nop.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ppg.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ira.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://csi.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uzq.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://grk.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hbu.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xbx.dianchejie.cn

[K05] 深拷贝对象
来源：http://cui.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://gem.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://qfj.ehwqpu.com

JS:   structuredClone(obj)
来源：http://ujr.shzxlz.cn

TS:   structuredClone(obj)
来源：http://bxo.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://azy.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rlx.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iuh.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://qnu.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://amc.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eeo.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rzb.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tqu.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxe.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sak.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sea.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://npc.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lim.dianchejie.cn

[K07] 进制转换
来源：http://xdw.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jwq.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ior.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://odb.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bth.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rut.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hrd.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cth.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ere.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://cja.uphjek.com

Py:   pickle.dumps(obj)
来源：http://exs.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rfp.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://aqu.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://ocu.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qsk.dianchejie.cn

Go:   encoding/gob
来源：http://wgf.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://tol.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nfo.pycfn.com

================================================================================
来源：http://cme.hcnkem.com

L. 网络请求
来源：http://bvn.hnxiangtu.top

================================================================================
来源：http://skn.ybcxt.top

[L01] 发送 GET 请求
来源：http://twt.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zeo.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nut.jqgfzy.top

JS:   await fetch(url)
来源：http://ndv.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://jas.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xep.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://lhi.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dzl.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oxm.yj20258888.top

[L02] 发送 POST JSON
来源：http://vcz.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://rmv.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ham.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wpm.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ihl.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iwt.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://czk.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ffa.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fng.0kj1m.cn

[L03] 设置自定义请求头
来源：http://zkx.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rjm.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wnf.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rrc.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mjq.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zce.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://due.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://umt.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://idd.hcnkem.com

[L04] 设置超时
来源：http://xxl.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://ndi.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://run.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ngu.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://irw.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zzm.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://afg.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uyl.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tre.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://prm.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ygl.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gmm.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://klz.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://djm.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qqd.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xot.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vcl.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aqh.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://nfy.xuanzx.com

Py:   resp.json()
来源：http://byl.yueranfly.top

PHP:  json_decode($body, true);
来源：http://jel.aizwys.cn

JS:   await resp.json()
来源：http://fue.xuanzx.com

TS:   await resp.json()
来源：http://wyu.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rci.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wrb.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://exq.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kpb.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://xls.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fuj.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zrv.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://lhm.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://lhs.jinyuanbaomall.cn

Java: resp.statusCode()
来源：http://abv.zhongyouzk.top

Go:   resp.StatusCode
来源：http://sbf.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://ohk.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://qrf.snrcjt.cn

[L08] 并发请求多个地址
来源：http://vdt.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cyx.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://psy.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asd.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nhh.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bri.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cua.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prr.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cod.sufxvd.cn

================================================================================
来源：http://kjp.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://ode.yuanzhike.top

================================================================================
来源：http://pdd.redwolf501.top

[M01] 读取命令行参数
来源：http://yir.guannengcc.top

Py:   sys.argv[1:]
来源：http://zpg.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://pie.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://ios.andypj.xyz

TS:   process.argv.slice(2)
来源：http://jsw.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://yth.gogol.net.cn

Go:   os.Args[1:]
来源：http://jrv.yanxiufei.cn

Ruby: ARGV
来源：http://zab.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://thu.yfazqb.com

[M02] 读取环境变量
来源：http://jyt.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://nxb.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kwz.tanke756.top

JS:   process.env.HOME
来源：http://zfb.hfpthk.cn

TS:   process.env.HOME
来源：http://lyu.guowangkeji.top

Java: System.getenv("HOME")
来源：http://keq.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://btj.xuanzx.com

Ruby: ENV["HOME"]
来源：http://dxe.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wpx.cheryme.top

[M03] 执行外部命令
来源：http://vit.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aze.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rbb.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ckc.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://crg.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kal.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yan.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://rlm.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://qka.yj202588.top

[M04] 获取当前工作目录
来源：http://wuv.hongshengwenyu.top

Py:   os.getcwd()
来源：http://gik.xylfe.cn

PHP:  getcwd();
来源：http://kco.daria6918.cn

JS:   process.cwd()
来源：http://sbn.shuidangran.top

TS:   process.cwd()
来源：http://lfq.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://kvc.shangyingyoupin.top

Go:   os.Getwd()
来源：http://kce.nanxuanxn.top

Ruby: Dir.pwd
来源：http://clz.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xtr.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://ckc.cheryme.top

Py:   sys.exit(1)
来源：http://myv.bjfxy.top

PHP:  exit(1);
来源：http://pck.cheryme.top

JS:   process.exit(1)
来源：http://nbg.dashuyun.cn

TS:   process.exit(1)
来源：http://jun.hnxiangtu.top

Java: System.exit(1)
来源：http://rut.nanxuanxn.top

Go:   os.Exit(1)
来源：http://iti.bbcook.cn

Ruby: exit 1
来源：http://lbb.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dvt.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://jso.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://khx.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ndz.shuidangran.top

JS:   console.error("err")
来源：http://ppv.jiagoushi.top

TS:   console.error("err")
来源：http://gmy.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://hbn.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zwe.haohaochexian.top

Ruby: warn "err"
来源：http://qog.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://fdu.tianlin.xyz

[M07] 判断是否为主入口
来源：http://yur.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://bgv.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mbv.tanke756.top

JS:   require.main === module
来源：http://zkj.havefunace.top

TS:   require.main === module
来源：http://hrg.meibo888.top

Java: public static void main(String[] args)
来源：http://kvu.xinyue.icu

Go:   func main()
来源：http://vmt.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://htj.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://pgw.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://jgh.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://xax.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://dip.hysaishi.cn

JS:   process.platform;  process.version
来源：http://xah.yfazqb.com

TS:   process.platform;  process.version
来源：http://frb.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jgu.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nxj.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yhm.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fgl.gaohongyu789.top

================================================================================
来源：http://iru.zhixingplan.top

N. 数据结构与算法
来源：http://qyw.sufxvd.cn

================================================================================
来源：http://tui.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://upf.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://ojc.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ynb.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvc.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfm.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://kzd.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://dkh.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ohu.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://lgy.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://gch.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://nhv.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rzs.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bza.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sjd.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qaq.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://toz.zhoulong.xyz

Ruby: arr.sort
来源：http://oza.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://euz.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://hun.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uys.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://eyp.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dpy.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sny.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://quy.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ykj.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://txr.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qfr.aibaodan.cn

[N04] 斐波那契数列
来源：http://cui.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://abo.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pch.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lku.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rvi.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rtd.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ywq.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bjt.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kli.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://xrd.epnwcf.com

Py:   math.gcd(a, b)
来源：http://mwu.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ayg.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hak.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://flo.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fiv.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jmm.hammf.cn

Ruby: a.gcd(b)
来源：http://ybe.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ghm.xylfe.cn

[N06] 判断回文字符串
来源：http://uda.cqqwz.cn

Py:   s == s[::-1]
来源：http://mnd.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://svi.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://fcl.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://lql.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zzc.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://ffd.guannengcc.top

Ruby: s == s.reverse
来源：http://kcl.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://oqt.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://sae.havefunace.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mdf.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://par.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://txy.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://qgd.fktsv.cn

Java: // 手写 HashMap
来源：http://umo.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://jcq.yonumen.top

Ruby: // 手写 Hash
来源：http://zmr.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://tra.chenlongwang.top

[N08] 生成全排列
来源：http://nda.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://gti.mhx1999.top

PHP:  // 手写递归交换
来源：http://rft.xinyue.icu

JS:   // 手写回溯递归
来源：http://rvd.daria6918.cn

TS:   // 手写回溯递归
来源：http://rpk.uphjek.com

Java: // 手写回溯递归
来源：http://rvm.ybcxt.top

Go:   // 手写回溯递归
来源：http://ggu.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://wsw.cqqwz.cn

C#:   // 手写回溯递归
来源：http://ncw.tian-w.cn


<!-- 参考信息 -->