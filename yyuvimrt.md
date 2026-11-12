代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cbk.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bvg.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zvl.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://yac.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://boc.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vey.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://umq.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dmu.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qgb.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://emd.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hgy.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://prb.daria6918.cn

================================================================================
来源：http://xpt.tian-w.cn

K. JSON 与序列化
来源：http://nul.hysaishi.cn

================================================================================
来源：http://aca.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://fxx.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lgw.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://trc.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://gpn.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://hja.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://row.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://sjl.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zxh.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kvt.xinyue.icu

[K02] JSON 字符串转对象
来源：http://ana.yj20258.top

Py:   json.loads(s)
来源：http://fey.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mrs.cheryme.top

JS:   JSON.parse(s)
来源：http://wcy.svipenyu.cn

TS:   JSON.parse(s)
来源：http://zem.svipenyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://epz.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://hmv.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://gid.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vfe.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://xri.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sfe.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wof.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ckc.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kec.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://htp.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yyv.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nqb.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uok.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://qey.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfw.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aoz.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qcb.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tqc.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ryd.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nxq.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rkw.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ehw.yangfankeji.com

[K05] 深拷贝对象
来源：http://qym.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://hii.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://dxg.zycfv.cn

JS:   structuredClone(obj)
来源：http://jkt.bjfxy.top

TS:   structuredClone(obj)
来源：http://jjv.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jpl.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://glf.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xmo.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mbu.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://sky.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cqf.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dal.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rnd.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfz.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lmx.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://sep.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vom.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://roe.yvedp.cn

[K07] 进制转换
来源：http://sbv.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://srd.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mit.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jmk.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yla.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lqh.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pkl.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fjq.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gbk.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://crz.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://lmu.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lud.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://lnp.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://ncy.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bij.zhijiandao.cn

Go:   encoding/gob
来源：http://uci.jinqigfzy.top

Ruby: Marshal.dump(obj)
来源：http://gmw.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yjk.jinghuilouyu.cn

================================================================================
来源：http://drz.epnwcf.com

L. 网络请求
来源：http://jgi.jianghu66.top

================================================================================
来源：http://dba.xuanzx.com

[L01] 发送 GET 请求
来源：http://tkw.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ysh.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dic.sweek.top

JS:   await fetch(url)
来源：http://qsg.fengsongda.top

TS:   await fetch(url)
来源：http://haz.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qvt.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://lfx.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rpq.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bvt.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://ovd.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rmm.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tas.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fig.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mmh.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zzd.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nas.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sjk.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fwj.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://rdc.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hcc.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dbg.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nya.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tih.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iry.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wms.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ynn.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kdb.316326.xyz

[L04] 设置超时
来源：http://tan.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://zpe.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ard.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lca.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vsw.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kee.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wcm.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mor.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fxg.yueranfly.top

[L05] 上传文件（multipart）
来源：http://zhp.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jpt.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xrf.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://obl.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hvm.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wxs.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kbz.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ysv.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uhm.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://kuq.yueranfly.top

Py:   resp.json()
来源：http://hyu.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://xsp.sxryk.cn

JS:   await resp.json()
来源：http://vwj.xinyue.icu

TS:   await resp.json()
来源：http://afx.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hnu.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bpy.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://bzv.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zkx.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://izx.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wqc.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yql.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://uma.sweek.top

TS:   resp.ok;  resp.status
来源：http://iys.jlsjyb.cn

Java: resp.statusCode()
来源：http://nhx.pycfn.com

Go:   resp.StatusCode
来源：http://dvl.yuanzhike.top

Ruby: resp.code.to_i
来源：http://xsd.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://aek.yvedp.cn

[L08] 并发请求多个地址
来源：http://eto.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gpz.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://pgg.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://thh.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cak.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tud.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://shp.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ykf.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xsd.yonumen.top

================================================================================
来源：http://kye.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://rac.hnqzz.top

================================================================================
来源：http://hjh.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://qng.svipenyu.cn

Py:   sys.argv[1:]
来源：http://ist.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://qha.xylfe.cn

JS:   process.argv.slice(2)
来源：http://qhc.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://qjo.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://cdi.sufxvd.cn

Go:   os.Args[1:]
来源：http://mwc.hnxiangtu.top

Ruby: ARGV
来源：http://rek.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://udk.gaohongyu789.top

[M02] 读取环境变量
来源：http://shi.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://nmy.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://omi.tian-w.cn

JS:   process.env.HOME
来源：http://hbd.dashuyun.cn

TS:   process.env.HOME
来源：http://zwj.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://icc.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aga.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://sqb.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rzy.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://dey.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xzq.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lqc.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://abg.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://kas.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jhi.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nls.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pre.fktsv.cn

C#:   Process.Start("ls", "-l");
来源：http://ult.zhengqikj.top

[M04] 获取当前工作目录
来源：http://etc.gaohongyu789.top

Py:   os.getcwd()
来源：http://oss.cheryme.top

PHP:  getcwd();
来源：http://alh.yangfankeji.com

JS:   process.cwd()
来源：http://bpo.cheryme.top

TS:   process.cwd()
来源：http://hpa.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://hnn.hysaishi.cn

Go:   os.Getwd()
来源：http://xxf.tanke756.top

Ruby: Dir.pwd
来源：http://qbm.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xks.chenjidiqi.icu

[M05] 设置退出码
来源：http://xku.cdnleiting.top

Py:   sys.exit(1)
来源：http://ypg.fehbvm.com

PHP:  exit(1);
来源：http://lyc.aibaodan.cn

JS:   process.exit(1)
来源：http://jnv.svipenyu.cn

TS:   process.exit(1)
来源：http://rst.pycfn.com

Java: System.exit(1)
来源：http://him.guowangkeji.top

Go:   os.Exit(1)
来源：http://jbf.yj20258888.top

Ruby: exit 1
来源：http://sui.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ekg.yanxiufei.cn

[M06] 向标准错误输出
来源：http://gsx.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://kjy.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://enf.daria6918.cn

JS:   console.error("err")
来源：http://nls.sxryk.cn

TS:   console.error("err")
来源：http://ymm.vehdjk.com

Java: System.err.println("err")
来源：http://htf.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kxn.havefunace.top

Ruby: warn "err"
来源：http://sfm.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://qyh.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://dub.cheryme.top

Py:   if __name__ == "__main__":
来源：http://llx.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jdj.xuetiantiany.cn

JS:   require.main === module
来源：http://vsq.gaohongyu789.top

TS:   require.main === module
来源：http://eaz.gogol.net.cn

Java: public static void main(String[] args)
来源：http://alg.daria6918.cn

Go:   func main()
来源：http://qsy.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wfu.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://rmc.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://kzf.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://ypf.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://lbx.iojbl.cn

JS:   process.platform;  process.version
来源：http://nbx.zhixingplan.top

TS:   process.platform;  process.version
来源：http://iji.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gav.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qan.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wkv.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://std.birdmap.top

================================================================================
来源：http://zho.shuidangran.top

N. 数据结构与算法
来源：http://vmh.ctjpmb.com

================================================================================
来源：http://soe.tarul.cn

[N01] 二分查找（有序数组）
来源：http://bpi.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://prh.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vjs.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pnn.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zps.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://uwv.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://upd.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uwg.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://fov.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://ypd.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://enu.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rrz.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hhd.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aoc.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jsx.tian-w.cn

Go:   slices.Sort(arr)
来源：http://mos.aizwys.cn

Ruby: arr.sort
来源：http://xtf.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ryu.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://fvo.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jjq.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://cek.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jzc.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hcl.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ujn.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rtu.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dwc.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uqt.guowangkeji.top

[N04] 斐波那契数列
来源：http://ptb.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nap.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yzl.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gmh.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://stu.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vpb.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tdx.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zom.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ent.ydzc1.top

[N05] 最大公约数
来源：http://tod.sxryk.cn

Py:   math.gcd(a, b)
来源：http://cew.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rex.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jtg.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqp.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://shv.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mhr.zdqjudy.top

Ruby: a.gcd(b)
来源：http://jen.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kmp.cashguo.top

[N06] 判断回文字符串
来源：http://ujj.yanxiufei.cn

Py:   s == s[::-1]
来源：http://ccg.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://bmc.epnwcf.com

JS:   s === [...s].reverse().join("")
来源：http://drj.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://oll.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wlc.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://zlc.jqgufenzy.top

Ruby: s == s.reverse
来源：http://avl.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ulk.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://asz.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nxg.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hom.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://obi.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://iwb.redwolf501.top

Java: // 手写 HashMap
来源：http://gyr.redwolf501.top


<!-- 参考信息 -->