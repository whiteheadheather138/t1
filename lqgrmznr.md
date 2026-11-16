代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://aie.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gzr.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://udo.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mtx.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xpx.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cpr.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tii.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uox.hnqzz.top

================================================================================
来源：http://gfn.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://ojk.gotoacloud.top

================================================================================
来源：http://cew.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://lqb.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gpj.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jzr.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://uhy.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://pxb.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pak.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://cdt.gogol.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zvu.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kmw.epnwcf.com

[K02] JSON 字符串转对象
来源：http://zsm.jiagoushi.top

Py:   json.loads(s)
来源：http://pwo.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rzn.vehdjk.com

JS:   JSON.parse(s)
来源：http://wly.shuidangran.top

TS:   JSON.parse(s)
来源：http://gxq.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sxc.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://ojo.guannengcc.top

Ruby: JSON.parse(s)
来源：http://ovm.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://slm.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://mkx.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yoz.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lzs.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gxw.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vtg.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://liy.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qvs.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://rjy.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cru.hammf.cn

[K04] 读取 JSON 文件
来源：http://kvt.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bny.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qqu.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oeu.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pkx.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qgj.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hhp.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vxu.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jxa.tian-w.cn

[K05] 深拷贝对象
来源：http://ouk.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://tge.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://lhz.hammf.cn

JS:   structuredClone(obj)
来源：http://fac.bjfxy.top

TS:   structuredClone(obj)
来源：http://npr.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sap.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bup.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://teq.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hnb.hnqzz.top

[K06] 解析 URL 查询串
来源：http://eeq.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jfz.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jes.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lfd.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ixw.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cip.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://krp.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sgr.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zco.jyoumei.cn

[K07] 进制转换
来源：http://xue.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mnd.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hdh.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mgc.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqa.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lac.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tsl.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ysk.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jww.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://fvg.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://rqw.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ljd.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://kcx.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://rhn.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://frc.redwolf501.top

Go:   encoding/gob
来源：http://bzu.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://coz.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kgp.zhixingplan.top

================================================================================
来源：http://rex.ctjpmb.com

L. 网络请求
来源：http://pbz.mhx1999.top

================================================================================
来源：http://qus.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://bjo.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sud.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://deu.iojbl.cn

JS:   await fetch(url)
来源：http://cen.bjfxy.top

TS:   await fetch(url)
来源：http://qbs.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qcz.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://cxk.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://hhx.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jab.xziqi.cn

[L02] 发送 POST JSON
来源：http://ijk.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pjq.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wno.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gbz.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zht.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zmp.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mlw.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pwo.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qaz.iojbl.cn

[L03] 设置自定义请求头
来源：http://iyh.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ynn.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gjq.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zym.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rqf.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eqp.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ovd.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jiw.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yqk.xylfe.cn

[L04] 设置超时
来源：http://nui.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://rbf.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pnh.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://imw.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mum.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vvq.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vuj.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vnn.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yaf.pycfn.com

[L05] 上传文件（multipart）
来源：http://ylj.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://thb.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xhs.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ggm.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://efm.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nvx.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rqs.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vig.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fxy.sysykeji.top

[L06] 解析响应为 JSON
来源：http://naw.wangdashe.top

Py:   resp.json()
来源：http://hex.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://evj.svipenyu.cn

JS:   await resp.json()
来源：http://xnz.gzhubu.top

TS:   await resp.json()
来源：http://zio.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ytj.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mqv.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://pbp.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tsv.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://rgp.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nlo.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jgx.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://gge.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://gsc.9152youxi.cn

Java: resp.statusCode()
来源：http://bpf.hysaishi.cn

Go:   resp.StatusCode
来源：http://ohl.nwbrower.top

Ruby: resp.code.to_i
来源：http://omt.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://qwp.dashuyun.cn

[L08] 并发请求多个地址
来源：http://cpn.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oyh.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://vde.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://igc.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://was.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xqv.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://caw.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://btz.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhh.jinyuanbaomall.cn

================================================================================
来源：http://ado.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://zpy.gzhubu.top

================================================================================
来源：http://pig.yj202588.top

[M01] 读取命令行参数
来源：http://wuv.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://jvs.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://svn.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://iiq.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://tqk.yj202588.top

Java: args 数组（main 方法参数）
来源：http://yex.vehdjk.com

Go:   os.Args[1:]
来源：http://zez.ehwqpu.com

Ruby: ARGV
来源：http://gyr.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://kym.jqgufenzy.top

[M02] 读取环境变量
来源：http://odo.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://ubm.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sxy.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://fcc.epnwcf.com

TS:   process.env.HOME
来源：http://tam.hcnkem.com

Java: System.getenv("HOME")
来源：http://iqp.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yiy.tarul.cn

Ruby: ENV["HOME"]
来源：http://dfl.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zzg.yj202588.top

[M03] 执行外部命令
来源：http://diz.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ibt.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cax.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mcc.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tjj.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jhd.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://nla.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pex.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://mmq.yfazqb.com

[M04] 获取当前工作目录
来源：http://drl.dianchejie.cn

Py:   os.getcwd()
来源：http://iuz.zycfv.cn

PHP:  getcwd();
来源：http://vyl.bjfxy.top

JS:   process.cwd()
来源：http://rrx.xylfe.cn

TS:   process.cwd()
来源：http://bwp.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://rdj.daria6918.cn

Go:   os.Getwd()
来源：http://utk.haohaochexian.top

Ruby: Dir.pwd
来源：http://jhe.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://qvs.cashguo.top

[M05] 设置退出码
来源：http://nvu.zhongyouzk.top

Py:   sys.exit(1)
来源：http://dah.fehbvm.com

PHP:  exit(1);
来源：http://yhy.guannengcc.top

JS:   process.exit(1)
来源：http://evs.0kj1m.cn

TS:   process.exit(1)
来源：http://rqu.jinqigfzy.top

Java: System.exit(1)
来源：http://oan.cdnleiting.top

Go:   os.Exit(1)
来源：http://vss.guannengcc.top

Ruby: exit 1
来源：http://bsq.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kku.jinqigufen.top

[M06] 向标准错误输出
来源：http://osk.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://fiq.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bfg.shanyushiyangtech.top

JS:   console.error("err")
来源：http://xtp.cashguo.top

TS:   console.error("err")
来源：http://shc.hfpthk.cn

Java: System.err.println("err")
来源：http://cqc.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://avv.zdbjq.cn

Ruby: warn "err"
来源：http://sys.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://oql.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://ins.meibo888.top

Py:   if __name__ == "__main__":
来源：http://lpb.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vgi.uphjek.com

JS:   require.main === module
来源：http://ysy.tanke756.top

TS:   require.main === module
来源：http://nfa.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://yzo.sweek.top

Go:   func main()
来源：http://dyc.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://icw.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://zds.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://gyg.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://wuu.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://jef.uphjek.com

JS:   process.platform;  process.version
来源：http://udw.shuidangran.top

TS:   process.platform;  process.version
来源：http://tzs.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hon.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pdt.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lmi.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vgs.xinyue.icu

================================================================================
来源：http://ncb.zdqjudy.top

N. 数据结构与算法
来源：http://wut.cucudq.cn

================================================================================
来源：http://wdj.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://raz.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://fxf.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wcm.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iok.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bvv.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://tvo.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://coq.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zrs.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://xqv.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://rfy.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://iaw.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://irr.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxe.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://efy.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://afd.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://jov.chenzaomai.com

Ruby: arr.sort
来源：http://odi.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pbz.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://afa.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://leo.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://zcr.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbe.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zkg.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ugz.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fei.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fac.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://aqb.zdqjudy.top

[N04] 斐波那契数列
来源：http://mqb.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jmz.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qax.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysk.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fko.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xge.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ruv.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hdx.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xwd.dashuyun.cn

[N05] 最大公约数
来源：http://shp.daria6918.cn

Py:   math.gcd(a, b)
来源：http://wxx.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqz.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gns.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixm.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bhr.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lif.pycfn.com

Ruby: a.gcd(b)
来源：http://uco.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bob.fktsv.cn

[N06] 判断回文字符串
来源：http://qza.chenzaomai.com

Py:   s == s[::-1]
来源：http://wuj.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://cpb.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://boz.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://vva.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://myv.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://whs.yvedp.cn

Ruby: s == s.reverse
来源：http://dgk.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mhu.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://etb.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://idk.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rsp.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mey.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://byk.gotoacloud.top

Java: // 手写 HashMap
来源：http://rfk.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://abi.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://fcq.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qkw.cashguo.top

[N08] 生成全排列
来源：http://qak.yangfankeji.com


<!-- 参考信息 -->