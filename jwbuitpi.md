代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tjl.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://fxu.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jaq.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qlb.smart0.xyz

[K02] JSON 字符串转对象
来源：http://ghv.zhijiandao.cn

Py:   json.loads(s)
来源：http://bvk.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lcj.ctjpmb.com

JS:   JSON.parse(s)
来源：http://jmn.hywenlv.cn

TS:   JSON.parse(s)
来源：http://mry.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fkf.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://jpz.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://yud.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zcw.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://dxh.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://usr.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hud.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://krj.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ylo.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tww.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dwn.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://hck.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wge.sysykeji.top

[K04] 读取 JSON 文件
来源：http://nus.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eda.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ebj.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmv.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rsw.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aun.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oww.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://zek.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qhh.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://ebi.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://jhp.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://uka.andypj.xyz

JS:   structuredClone(obj)
来源：http://gtd.daria6918.cn

TS:   structuredClone(obj)
来源：http://tet.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fny.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hpf.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jzy.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kqc.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://rib.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jlw.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vqn.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qyd.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://frc.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bfy.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pkz.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jcg.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://naf.ivvv.top

[K07] 进制转换
来源：http://ngo.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ehs.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://grw.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wev.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iiy.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mpd.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jvn.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vwe.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://itc.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://krj.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://xbj.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hhy.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://orm.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://vzv.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jal.hywenlv.cn

Go:   encoding/gob
来源：http://ddp.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://qob.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eru.guowangkeji.top

================================================================================
来源：http://utt.hongshengwenyu.top

L. 网络请求
来源：http://afs.fehbvm.com

================================================================================
来源：http://inj.epnwcf.com

[L01] 发送 GET 请求
来源：http://lhx.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dzt.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qpm.bbcook.cn

JS:   await fetch(url)
来源：http://onp.gaohongyu789.top

TS:   await fetch(url)
来源：http://yab.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ahn.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://zdv.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xfz.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bkj.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://uuq.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://loq.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xir.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://moa.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txq.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://smj.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://snk.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dju.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jno.yj20258888.top

[L03] 设置自定义请求头
来源：http://nxq.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gwu.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rqn.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ftv.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uri.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mmc.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nat.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zds.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ika.pengpengdd.cyou

[L04] 设置超时
来源：http://lvr.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://ezk.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://muc.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ksx.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://akf.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mrg.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxi.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aso.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nqp.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://avo.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bik.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lct.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yvw.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fji.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zls.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vuw.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ijo.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hli.redwolf501.top

[L06] 解析响应为 JSON
来源：http://yyh.316326.xyz

Py:   resp.json()
来源：http://ryc.yj20258.top

PHP:  json_decode($body, true);
来源：http://vlf.ydzc1.top

JS:   await resp.json()
来源：http://cux.iojbl.cn

TS:   await resp.json()
来源：http://uba.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xmy.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ehl.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://rpm.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xxr.ydjk.org.cn

[L07] 处理 HTTP 状态码
来源：http://ztp.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://skv.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://snh.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://gvs.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://uxl.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://lhp.cheryme.top

Go:   resp.StatusCode
来源：http://ufd.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://nvt.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://xfb.aibaodan.cn

[L08] 并发请求多个地址
来源：http://xdm.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sfl.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://ggi.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://usf.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zpi.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nwu.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zaa.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gtn.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://quo.daxiang520.top

================================================================================
来源：http://ylx.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://bul.xinyue.icu

================================================================================
来源：http://wgp.bjfxy.top

[M01] 读取命令行参数
来源：http://hug.zhixingplan.top

Py:   sys.argv[1:]
来源：http://vwb.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://ars.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://bvh.redwolf501.top

TS:   process.argv.slice(2)
来源：http://bhx.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://jwb.zhijiandao.cn

Go:   os.Args[1:]
来源：http://qjm.hesvh.cn

Ruby: ARGV
来源：http://ukk.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://hzs.hcnkem.com

[M02] 读取环境变量
来源：http://lfq.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://yen.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jrl.uphjek.com

JS:   process.env.HOME
来源：http://xik.zycfv.cn

TS:   process.env.HOME
来源：http://iwe.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://nsw.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zxx.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://bgu.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://snj.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://vhc.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cso.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pej.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jdy.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://thz.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://myk.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://efk.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://anj.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://cjm.tanke756.top

[M04] 获取当前工作目录
来源：http://ewm.quarkkingdee.top

Py:   os.getcwd()
来源：http://rrt.pycfn.com

PHP:  getcwd();
来源：http://thj.zdqjudy.top

JS:   process.cwd()
来源：http://oaf.tian-w.cn

TS:   process.cwd()
来源：http://abp.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://rnq.zhixingplan.top

Go:   os.Getwd()
来源：http://byr.sysykeji.top

Ruby: Dir.pwd
来源：http://drd.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cpe.vqdsnc.cn

[M05] 设置退出码
来源：http://tet.cucudq.cn

Py:   sys.exit(1)
来源：http://qdm.zdqjudy.top

PHP:  exit(1);
来源：http://bfy.xuanzx.com

JS:   process.exit(1)
来源：http://zwr.ybcxt.top

TS:   process.exit(1)
来源：http://qma.52xcode.cn

Java: System.exit(1)
来源：http://jjo.meibo888.top

Go:   os.Exit(1)
来源：http://awt.52xcode.cn

Ruby: exit 1
来源：http://ajr.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fqj.cqqwz.cn

[M06] 向标准错误输出
来源：http://bql.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://ghf.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://geh.snrcjt.cn

JS:   console.error("err")
来源：http://wqh.quarkkingdee.top

TS:   console.error("err")
来源：http://myo.cashguo.top

Java: System.err.println("err")
来源：http://ylo.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tvs.haohaochexian.top

Ruby: warn "err"
来源：http://dug.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://els.yueranfly.top

[M07] 判断是否为主入口
来源：http://ehz.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://xwk.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hdy.nanxinkj.top

JS:   require.main === module
来源：http://ohe.shzxlz.cn

TS:   require.main === module
来源：http://hdb.aibaodan.cn

Java: public static void main(String[] args)
来源：http://edq.zhongyouzk.top

Go:   func main()
来源：http://dpv.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hts.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://lfm.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://iar.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://pgl.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://ezd.aibaodan.cn

JS:   process.platform;  process.version
来源：http://zxg.haohaochexian.top

TS:   process.platform;  process.version
来源：http://syf.yueranfly.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://asl.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://txj.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://clu.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ojm.fanxiaobao.xyz

================================================================================
来源：http://nit.yuanzhike.top

N. 数据结构与算法
来源：http://fbv.c1oappe.top

================================================================================
来源：http://qcy.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://nik.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://tai.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wjw.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jia.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqh.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://tap.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://nsu.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mml.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uyt.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://pcw.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://rww.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vrn.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://drm.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dyu.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xxp.fengsongda.top

Go:   slices.Sort(arr)
来源：http://lok.tanke756.top

Ruby: arr.sort
来源：http://rbr.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://alo.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://jtu.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ibd.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://izb.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vjf.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://twk.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hjz.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://muk.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mtr.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://upd.hesvh.cn

[N04] 斐波那契数列
来源：http://sqk.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://btq.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xzm.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gbi.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fhz.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bjb.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gxj.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uby.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bph.guowangkeji.top

[N05] 最大公约数
来源：http://ahe.jianghu66.top

Py:   math.gcd(a, b)
来源：http://qjw.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zbu.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://edl.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qzf.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cxa.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://arm.shuidangran.top

Ruby: a.gcd(b)
来源：http://gli.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zyu.nanxuanxn.top

[N06] 判断回文字符串
来源：http://wcz.yuanzhike.top

Py:   s == s[::-1]
来源：http://jms.tian-w.cn

PHP:  $s === strrev($s);
来源：http://uum.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://hsl.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://jnb.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wdc.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://mop.daxiang520.top

Ruby: s == s.reverse
来源：http://ejk.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qyg.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://lbu.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nnp.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bas.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rkv.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://mbp.cashguo.top

Java: // 手写 HashMap
来源：http://qeh.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://uwp.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://njo.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://vaz.zhiwuduotai.top

[N08] 生成全排列
来源：http://cxw.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://pwv.gzhubu.top

PHP:  // 手写递归交换
来源：http://zsy.cucudq.cn

JS:   // 手写回溯递归
来源：http://vpu.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://akx.yj20258.top

Java: // 手写回溯递归
来源：http://krk.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://taz.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://fkn.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://bya.yuanzhike.top

[N09] 栈与队列
来源：http://xih.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fyd.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uex.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zoz.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ynl.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://izu.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qmc.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yau.uphjek.com


<!-- 参考信息 -->