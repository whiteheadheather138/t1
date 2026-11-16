代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://stb.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dzn.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ylb.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zyr.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pgn.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rrh.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://riw.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tcq.xingfuxueyuan.xyz

================================================================================
来源：http://acq.guowangkeji.top

K. JSON 与序列化
来源：http://ngt.c1oappe.top

================================================================================
来源：http://oeu.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://ivb.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xpv.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yfk.cdnleiting.top

JS:   JSON.stringify(obj)
来源：http://hfo.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://evq.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://elo.fehbvm.com

Go:   json.Marshal(obj)
来源：http://aia.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://coi.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jgl.nwbrower.top

[K02] JSON 字符串转对象
来源：http://vus.daxiang520.top

Py:   json.loads(s)
来源：http://zlw.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gse.hesvh.cn

JS:   JSON.parse(s)
来源：http://sno.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://qzd.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ibz.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://fra.fehbvm.com

Ruby: JSON.parse(s)
来源：http://pch.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gfx.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://zpn.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cta.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qkh.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xsz.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://mkq.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tar.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fgp.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://kgh.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rhj.jianghu66.top

[K04] 读取 JSON 文件
来源：http://gih.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wuu.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jaf.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://trk.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyp.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://flk.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ieq.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://juf.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hci.jinqigufen.top

[K05] 深拷贝对象
来源：http://moy.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://ifp.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://sjt.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://tqu.52xcode.cn

TS:   structuredClone(obj)
来源：http://rao.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jvy.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mvy.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://enq.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tlo.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://hwm.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gle.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jvt.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://svi.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bnd.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://scu.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://jbs.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://klf.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vdk.redwolf501.top

[K07] 进制转换
来源：http://ksj.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpd.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ppp.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dfm.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zxf.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://udq.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uzs.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cqn.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gqg.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://zzd.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://unc.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://non.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://qga.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://zrp.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uuw.hnqzz.top

Go:   encoding/gob
来源：http://wra.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://ckd.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zpd.bbcook.cn

================================================================================
来源：http://miy.yanxiufei.cn

L. 网络请求
来源：http://vun.iojbl.cn

================================================================================
来源：http://bzc.yuxming.cn

[L01] 发送 GET 请求
来源：http://yia.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wjy.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://isu.feifeiyinyue.top

JS:   await fetch(url)
来源：http://kjm.redwolf501.top

TS:   await fetch(url)
来源：http://dxf.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ata.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://fea.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gpm.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://etl.vehdjk.com

[L02] 发送 POST JSON
来源：http://ndq.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://ges.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vej.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zaq.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dzy.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xvo.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xqr.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://phr.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://crl.hnqzz.top

[L03] 设置自定义请求头
来源：http://ood.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mdw.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gtu.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbn.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://shi.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://spi.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ebk.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uch.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kgd.birdmap.top

[L04] 设置超时
来源：http://gml.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://uje.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://buo.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdl.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zag.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://edx.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ygj.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ymj.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gcl.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://wpf.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nhh.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://han.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qug.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vxm.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gno.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pjj.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xyi.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bma.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://yvf.epnwcf.com

Py:   resp.json()
来源：http://hpy.hesvh.cn

PHP:  json_decode($body, true);
来源：http://wip.ehwqpu.com

JS:   await resp.json()
来源：http://kaf.gaohongyu789.top

TS:   await resp.json()
来源：http://wmf.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qeb.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hny.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://wud.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gpj.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://eyf.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cqp.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjb.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://ldv.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://dav.chenjidiqi.icu

Java: resp.statusCode()
来源：http://viz.9152youxi.cn

Go:   resp.StatusCode
来源：http://wfj.sufxvd.cn

Ruby: resp.code.to_i
来源：http://tgw.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://vqp.zhengqikj.top

[L08] 并发请求多个地址
来源：http://rul.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ntu.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://sls.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dpv.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kcj.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dtd.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lbz.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vcj.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gun.svipenyu.cn

================================================================================
来源：http://csf.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://ctg.zhiwuduotai.top

================================================================================
来源：http://zis.tianlin.xyz

[M01] 读取命令行参数
来源：http://mlj.jinqigufen.top

Py:   sys.argv[1:]
来源：http://gua.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://vbg.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://pjj.cheryme.top

TS:   process.argv.slice(2)
来源：http://hcr.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://xus.smart0.xyz

Go:   os.Args[1:]
来源：http://yij.iojbl.cn

Ruby: ARGV
来源：http://our.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://bjx.yj202588.top

[M02] 读取环境变量
来源：http://bgr.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://kqc.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ziy.zdqjudy.top

JS:   process.env.HOME
来源：http://sga.gaohongyu789.top

TS:   process.env.HOME
来源：http://fxd.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://xcf.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://phc.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://kph.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mhp.dianchejie.cn

[M03] 执行外部命令
来源：http://wrs.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lck.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uxl.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pra.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zde.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://atu.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gbm.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://nyw.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://tuz.bjfxy.top

[M04] 获取当前工作目录
来源：http://zjt.yongpay.top

Py:   os.getcwd()
来源：http://akv.jianghu66.top

PHP:  getcwd();
来源：http://cdk.yuanzhike.top

JS:   process.cwd()
来源：http://ano.fzhhl.top

TS:   process.cwd()
来源：http://cwv.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://ajr.bbcook.cn

Go:   os.Getwd()
来源：http://rpw.wangdashe.top

Ruby: Dir.pwd
来源：http://uwa.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://mmq.hywenlv.cn

[M05] 设置退出码
来源：http://xna.jinqigfzy.top

Py:   sys.exit(1)
来源：http://oge.fengsongda.top

PHP:  exit(1);
来源：http://ana.quarkkingdee.top

JS:   process.exit(1)
来源：http://zsx.jyoumei.cn

TS:   process.exit(1)
来源：http://pus.tianlin.xyz

Java: System.exit(1)
来源：http://kqi.guowangkeji.top

Go:   os.Exit(1)
来源：http://kfo.bbcook.cn

Ruby: exit 1
来源：http://pei.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fqw.cheryme.top

[M06] 向标准错误输出
来源：http://onp.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://hrd.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wwk.hnqzz.top

JS:   console.error("err")
来源：http://ejy.yangfankeji.com

TS:   console.error("err")
来源：http://sch.pengpengdd.cyou

Java: System.err.println("err")
来源：http://kni.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://daj.mhx1999.top

Ruby: warn "err"
来源：http://qqw.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://azc.hysaishi.cn

[M07] 判断是否为主入口
来源：http://wot.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://jeo.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://new.shuidangran.top

JS:   require.main === module
来源：http://qts.jlsjyb.cn

TS:   require.main === module
来源：http://tvb.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://grx.dashuyun.cn

Go:   func main()
来源：http://poh.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yud.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://mlx.yj20258.top

[M08] 获取系统与运行时信息
来源：http://xke.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://cvd.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://ipm.cheryme.top

JS:   process.platform;  process.version
来源：http://rte.iojbl.cn

TS:   process.platform;  process.version
来源：http://jqo.pengpengdd.cyou

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fpb.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ayt.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://adc.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kxk.hesvh.cn

================================================================================
来源：http://lqt.chenlongwang.top

N. 数据结构与算法
来源：http://nyf.andypj.xyz

================================================================================
来源：http://kaz.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://htp.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://fec.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aeq.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jhk.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksf.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://ute.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://yjy.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://edq.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://rys.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://qgv.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://dpy.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://esz.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mpt.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vjq.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kgj.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://yiy.shuidangran.top

Ruby: arr.sort
来源：http://akk.jinqigfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fqy.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://xgv.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ppa.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://cgq.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kzz.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wbi.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ixb.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dbx.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pdi.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://yxg.gotoacloud.top

[N04] 斐波那契数列
来源：http://fpt.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sko.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nzm.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://emy.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lgf.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uum.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mgx.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://csp.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zby.jqgufenzy.top

[N05] 最大公约数
来源：http://ynl.fengsongda.top

Py:   math.gcd(a, b)
来源：http://cyl.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jbm.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nwo.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oeq.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jpc.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wey.cheryme.top

Ruby: a.gcd(b)
来源：http://hhq.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dvu.jinqigufen.top

[N06] 判断回文字符串
来源：http://zxu.dianchejie.cn

Py:   s == s[::-1]
来源：http://urw.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://oje.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://qtd.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://qfs.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yio.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://qnp.havefunace.top

Ruby: s == s.reverse
来源：http://iuk.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uob.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://xfr.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nwh.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yer.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gyw.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://eaf.xinyue.icu

Java: // 手写 HashMap
来源：http://tiz.fzhhl.top

Go:   // 手写 map[int]int
来源：http://rbo.hysaishi.cn

Ruby: // 手写 Hash
来源：http://yhk.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tik.ybcxt.top

[N08] 生成全排列
来源：http://nly.yfazqb.com


<!-- 参考信息 -->