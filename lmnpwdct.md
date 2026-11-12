代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vom.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rql.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://alp.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qoh.ctjpmb.com

================================================================================
来源：http://oda.cdnleiting.top

K. JSON 与序列化
来源：http://sfd.zdqjudy.top

================================================================================
来源：http://xtz.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://sre.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://awk.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wro.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://ghy.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://mqv.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aed.xuanzx.com

Go:   json.Marshal(obj)
来源：http://xwe.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://gtr.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://htn.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://hco.redwolf501.top

Py:   json.loads(s)
来源：http://xfx.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nyp.zycfv.cn

JS:   JSON.parse(s)
来源：http://tde.zhixingplan.top

TS:   JSON.parse(s)
来源：http://tif.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jgh.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://usj.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://hzy.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lbj.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://lpl.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fei.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eva.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qqw.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mzu.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lgw.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hwu.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://seq.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://acn.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://anq.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wpo.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vis.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vew.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ily.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ngm.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://emy.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://agy.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://piw.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://kal.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://unn.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://rkc.xziqi.cn

JS:   structuredClone(obj)
来源：http://irq.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://anq.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eob.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fgc.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uhu.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://umk.wangdashe.top

[K06] 解析 URL 查询串
来源：http://cup.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tiy.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://flc.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://plt.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jbp.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aof.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qfx.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bne.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ndv.hnxiangtu.top

[K07] 进制转换
来源：http://krv.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yss.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uwl.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://owt.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zhg.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bwf.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vgw.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vow.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vgw.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://wpz.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://mkw.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wvr.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://icb.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://wvl.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jet.daria6918.cn

Go:   encoding/gob
来源：http://dkj.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://tdb.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yik.sxryk.cn

================================================================================
来源：http://hmw.chenjidiqi.icu

L. 网络请求
来源：http://thw.tian-w.cn

================================================================================
来源：http://qbc.yonumen.top

[L01] 发送 GET 请求
来源：http://vmc.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rtx.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xdb.meibo888.top

JS:   await fetch(url)
来源：http://geu.cqqwz.cn

TS:   await fetch(url)
来源：http://tga.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://efm.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://nxv.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ftn.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jbl.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://jhh.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qbs.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://taz.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://off.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lbf.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ejm.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://omz.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rwz.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mmh.fengsongda.top

[L03] 设置自定义请求头
来源：http://oaj.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hiy.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mwa.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mfb.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hil.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uoy.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vrf.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xas.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://swt.gaohongyu789.top

[L04] 设置超时
来源：http://dbf.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://aui.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ehq.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://amj.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lms.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dfw.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mem.yj202588.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ztt.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kvq.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://oue.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fgb.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vhq.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ghm.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rfs.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sgn.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bvh.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ilh.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pqm.jqgfzy.top

[L06] 解析响应为 JSON
来源：http://wtj.ctjpmb.com

Py:   resp.json()
来源：http://diq.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://djy.sjlbkw.cn

JS:   await resp.json()
来源：http://mir.sufxvd.cn

TS:   await resp.json()
来源：http://pgu.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://thx.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zhd.hcnkem.com

Ruby: JSON.parse(resp.body)
来源：http://xah.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yfn.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://ynn.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wxn.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lyb.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://xnh.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://gxd.yuanzhike.top

Java: resp.statusCode()
来源：http://oma.tarul.cn

Go:   resp.StatusCode
来源：http://mrr.yj20258888.top

Ruby: resp.code.to_i
来源：http://dof.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://ufv.aizwys.cn

[L08] 并发请求多个地址
来源：http://asr.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pwe.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://gua.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qrr.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oop.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ovy.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tmi.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ftb.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mct.snrcjt.cn

================================================================================
来源：http://oce.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://pfp.yonumen.top

================================================================================
来源：http://kcc.xziqi.cn

[M01] 读取命令行参数
来源：http://sql.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://tky.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://qcl.iojbl.cn

JS:   process.argv.slice(2)
来源：http://ivx.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://qoh.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://has.gaohongyu789.top

Go:   os.Args[1:]
来源：http://zwj.wangdashe.top

Ruby: ARGV
来源：http://mhz.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://cor.hcnkem.com

[M02] 读取环境变量
来源：http://eeb.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://ngs.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sva.hongshengwenyu.top

JS:   process.env.HOME
来源：http://het.hywenlv.cn

TS:   process.env.HOME
来源：http://vqi.epnwcf.com

Java: System.getenv("HOME")
来源：http://uom.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vbf.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://huq.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tig.guowangkeji.top

[M03] 执行外部命令
来源：http://aof.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://btf.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vht.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vdi.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://exb.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://upn.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://byw.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://opk.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://uce.yfazqb.com

[M04] 获取当前工作目录
来源：http://mlb.jinqigfzy.top

Py:   os.getcwd()
来源：http://vzi.chenzaomai.com

PHP:  getcwd();
来源：http://srb.xuanzx.com

JS:   process.cwd()
来源：http://dqk.bjfxy.top

TS:   process.cwd()
来源：http://syu.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://gwn.shuidangran.top

Go:   os.Getwd()
来源：http://pab.snrcjt.cn

Ruby: Dir.pwd
来源：http://zub.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://eca.meibo888.top

[M05] 设置退出码
来源：http://evp.tarul.cn

Py:   sys.exit(1)
来源：http://rnj.shzxlz.cn

PHP:  exit(1);
来源：http://vlg.yfazqb.com

JS:   process.exit(1)
来源：http://emc.sjlbkw.cn

TS:   process.exit(1)
来源：http://oan.aibaodan.cn

Java: System.exit(1)
来源：http://iiu.svipenyu.cn

Go:   os.Exit(1)
来源：http://cta.yanxiufei.cn

Ruby: exit 1
来源：http://goa.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gfy.52xcode.cn

[M06] 向标准错误输出
来源：http://zbw.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://skh.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oba.zhiwuduotai.top

JS:   console.error("err")
来源：http://mpk.cashguo.top

TS:   console.error("err")
来源：http://fuw.zhijiandao.cn

Java: System.err.println("err")
来源：http://nvv.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xjr.birdmap.top

Ruby: warn "err"
来源：http://rwx.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://qfo.nwbrower.top

[M07] 判断是否为主入口
来源：http://wtx.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://hko.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mtk.guowangkeji.top

JS:   require.main === module
来源：http://zyd.bbcook.cn

TS:   require.main === module
来源：http://qje.yangfankeji.com

Java: public static void main(String[] args)
来源：http://alv.ehwqpu.com

Go:   func main()
来源：http://fat.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wcx.cashguo.top

C#:   static void Main(string[] args)
来源：http://ymv.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://nil.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://ghn.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://biz.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://jqz.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://czr.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zrp.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://xee.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gok.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jcr.fengsongda.top

================================================================================
来源：http://kbb.feifeiyinyue.top

N. 数据结构与算法
来源：http://oqk.yanxiufei.cn

================================================================================
来源：http://hvv.tanke756.top

[N01] 二分查找（有序数组）
来源：http://lno.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://ojm.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hen.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kry.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lvb.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://zkf.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://vlx.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://exy.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://shb.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://lzs.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://dwg.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ujz.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uxt.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gzy.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iwd.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://uuq.yanxiufei.cn

Ruby: arr.sort
来源：http://sph.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gdi.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://pil.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://duu.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://ikx.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wwz.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://egu.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gqj.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zef.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vqf.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://ang.jqgufenzy.top

[N04] 斐波那契数列
来源：http://ujb.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://loe.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://grr.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dsj.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nro.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://flh.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kwi.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://doj.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://czx.fzhhl.top

[N05] 最大公约数
来源：http://ykv.fengsongda.top

Py:   math.gcd(a, b)
来源：http://zmm.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hvj.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugq.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyn.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gtu.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tja.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://oyh.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sto.zhongyouzk.top

[N06] 判断回文字符串
来源：http://slq.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://uae.xziqi.cn

PHP:  $s === strrev($s);
来源：http://zfd.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://qqt.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://kxf.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nkr.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://tdc.yanxiufei.cn

Ruby: s == s.reverse
来源：http://cwb.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gny.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://txi.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zos.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zww.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mer.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://dhb.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://wxe.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://fob.haohaochexian.top

Ruby: // 手写 Hash
来源：http://dpf.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cll.ppjwa.cn

[N08] 生成全排列
来源：http://qnc.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://tpb.0kj1m.cn

PHP:  // 手写递归交换
来源：http://msk.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://rvi.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://ern.cucudq.cn


<!-- 参考信息 -->