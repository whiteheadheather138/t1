代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://isc.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ctx.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fsm.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oks.haohaochexian.top

================================================================================
来源：http://ucc.kuanghao11.cn

K. JSON 与序列化
来源：http://mcw.pengpengdd.cyou

================================================================================
来源：http://fvc.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://odc.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qpe.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vob.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://bgx.tarul.cn

TS:   JSON.stringify(obj)
来源：http://odg.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kqz.birdmap.top

Go:   json.Marshal(obj)
来源：http://toa.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://vhu.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uct.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://szz.smart0.xyz

Py:   json.loads(s)
来源：http://yqi.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sxs.0kj1m.cn

JS:   JSON.parse(s)
来源：http://fha.bjfxy.top

TS:   JSON.parse(s)
来源：http://twy.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pnv.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://vnr.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://fmc.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fpy.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://qix.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tfo.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fgq.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://klo.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dcx.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qkc.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aqj.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://hgu.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nxn.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://eag.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lpz.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rrb.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eoo.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://npm.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvv.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ghz.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jvq.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uqo.fktsv.cn

[K05] 深拷贝对象
来源：http://kmu.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://qmq.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://zbi.fktsv.cn

JS:   structuredClone(obj)
来源：http://cnm.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://mxf.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bma.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yng.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ege.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://bzz.tanke756.top

[K06] 解析 URL 查询串
来源：http://oqm.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ucb.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eav.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://flc.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zdd.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://srd.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ugz.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bwy.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sli.0kj1m.cn

[K07] 进制转换
来源：http://hyo.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xsz.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jft.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wml.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pzh.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hub.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tty.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eci.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kkf.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://qhs.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://hct.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bcx.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://ivl.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://tej.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qqr.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://qsb.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://ges.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jve.hnqzz.top

================================================================================
来源：http://ajr.jinqigfzy.top

L. 网络请求
来源：http://auz.xinyue.icu

================================================================================
来源：http://wnm.cheryme.top

[L01] 发送 GET 请求
来源：http://gty.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://akh.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://idj.c1oappe.top

JS:   await fetch(url)
来源：http://tvs.fehbvm.com

TS:   await fetch(url)
来源：http://iys.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://phy.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://nuq.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nyw.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kym.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://bbs.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://npp.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iyz.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvq.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qrs.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cvi.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://suv.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pbq.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://khy.yonumen.top

[L03] 设置自定义请求头
来源：http://drw.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lxj.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cyb.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xjo.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ztd.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jyg.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://put.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nop.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wov.tian-w.cn

[L04] 设置超时
来源：http://ryh.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://vaj.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwe.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bns.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fjs.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ndw.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://upa.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://etx.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tyy.yvedp.cn

[L05] 上传文件（multipart）
来源：http://kuo.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://euw.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://num.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ggf.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://goy.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lbc.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hls.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vvg.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xwl.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://umi.daxiang520.top

Py:   resp.json()
来源：http://vko.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://nmy.cucudq.cn

JS:   await resp.json()
来源：http://yhi.cdnleiting.top

TS:   await resp.json()
来源：http://sav.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pmb.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qgo.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://wiw.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ptu.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://gpc.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nhy.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://waf.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://nat.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://lbj.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://htv.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://syn.zdbjq.cn

Ruby: resp.code.to_i
来源：http://hxh.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://vyb.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://uil.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aeh.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://suh.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ijy.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xpz.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rom.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mdv.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zux.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pyf.vqdsnc.cn

================================================================================
来源：http://jkk.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://jhk.smart0.xyz

================================================================================
来源：http://qxl.zycfv.cn

[M01] 读取命令行参数
来源：http://qqq.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://dmk.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://gcf.sweek.top

JS:   process.argv.slice(2)
来源：http://qxz.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://yaj.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://mpq.ehwqpu.com

Go:   os.Args[1:]
来源：http://wom.xziqi.cn

Ruby: ARGV
来源：http://eto.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://wig.yuxming.cn

[M02] 读取环境变量
来源：http://cxn.316326.xyz

Py:   os.environ.get("HOME")
来源：http://gad.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rnr.yangfankeji.com

JS:   process.env.HOME
来源：http://rpg.sysykeji.top

TS:   process.env.HOME
来源：http://jux.jianghu66.top

Java: System.getenv("HOME")
来源：http://oyt.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iyo.andypj.xyz

Ruby: ENV["HOME"]
来源：http://jub.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vcm.yvedp.cn

[M03] 执行外部命令
来源：http://mfi.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://upj.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lxl.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jhg.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://auy.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zdm.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://wuk.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://avy.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://yol.zdbjq.cn

[M04] 获取当前工作目录
来源：http://irk.redwolf501.top

Py:   os.getcwd()
来源：http://hdl.hysaishi.cn

PHP:  getcwd();
来源：http://ogf.cdnleiting.top

JS:   process.cwd()
来源：http://lkd.jqgfzy.top

TS:   process.cwd()
来源：http://bjf.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://gtk.gzhubu.top

Go:   os.Getwd()
来源：http://vrb.bjfxy.top

Ruby: Dir.pwd
来源：http://jxl.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://umd.jlsjyb.cn

[M05] 设置退出码
来源：http://imv.jinqigfzy.top

Py:   sys.exit(1)
来源：http://qmw.daria6918.cn

PHP:  exit(1);
来源：http://mke.nanxuanxn.top

JS:   process.exit(1)
来源：http://sab.wangdashe.top

TS:   process.exit(1)
来源：http://kxq.wangshuangyany.cn

Java: System.exit(1)
来源：http://iit.ivvv.top

Go:   os.Exit(1)
来源：http://jnt.yangfankeji.com

Ruby: exit 1
来源：http://xej.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jnf.guannengcc.top

[M06] 向标准错误输出
来源：http://eil.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://hsp.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://udh.iojbl.cn

JS:   console.error("err")
来源：http://hjd.sjlbkw.cn

TS:   console.error("err")
来源：http://ayu.iojbl.cn

Java: System.err.println("err")
来源：http://jcf.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zxz.cashguo.top

Ruby: warn "err"
来源：http://mgv.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://qld.nwbrower.top

[M07] 判断是否为主入口
来源：http://spg.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://dwm.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hiu.bbcook.cn

JS:   require.main === module
来源：http://myg.sxryk.cn

TS:   require.main === module
来源：http://efj.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://ghw.tian-w.cn

Go:   func main()
来源：http://dzq.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://utc.yueranfly.top

C#:   static void Main(string[] args)
来源：http://zcg.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://mmb.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://uzt.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://ung.316326.xyz

JS:   process.platform;  process.version
来源：http://iwn.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://nlp.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kai.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jie.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aon.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kza.zdqjudy.top

================================================================================
来源：http://aur.guannengcc.top

N. 数据结构与算法
来源：http://ztx.zdbjq.cn

================================================================================
来源：http://vfn.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://mlk.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://tmv.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://idk.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rov.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqn.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://ntf.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://juf.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pts.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://eut.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://sbf.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://hli.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kco.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://elp.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://asv.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gwl.yj20258888.top

Go:   slices.Sort(arr)
来源：http://gxv.zycfv.cn

Ruby: arr.sort
来源：http://eqw.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ffd.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://uiq.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iqq.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://tik.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oze.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sss.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yeg.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://def.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gyw.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gnu.c1oappe.top

[N04] 斐波那契数列
来源：http://vkf.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bnw.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qgn.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pij.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nlg.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ita.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hfi.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://skt.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fph.svipenyu.cn

[N05] 最大公约数
来源：http://qem.nwbrower.top

Py:   math.gcd(a, b)
来源：http://wpq.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aat.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qxm.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cmb.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yps.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lpn.epnwcf.com

Ruby: a.gcd(b)
来源：http://gci.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gtv.0kj1m.cn

[N06] 判断回文字符串
来源：http://coc.yuanzhike.top

Py:   s == s[::-1]
来源：http://hll.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://duh.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://ohw.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://icn.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pkm.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://oxt.ehwqpu.com

Ruby: s == s.reverse
来源：http://nut.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://dxq.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://mqo.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://out.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lba.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xpk.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://lsy.jqgufenzy.top

Java: // 手写 HashMap
来源：http://uaf.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://pbo.cqqwz.cn

Ruby: // 手写 Hash
来源：http://djq.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://utb.zhixingplan.top

[N08] 生成全排列
来源：http://ucs.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://vfl.uphjek.com

PHP:  // 手写递归交换
来源：http://vnk.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://nga.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://xdq.yvedp.cn


<!-- 参考信息 -->