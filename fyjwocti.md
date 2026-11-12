代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://cnk.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lvk.gaohongyu789.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ikh.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dce.jiagoushi.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sfw.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://geo.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vsr.zhiwuduotai.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://klc.ybcxt.top

================================================================================
来源：http://sfa.hcnkem.com

K. JSON 与序列化
来源：http://eum.xuanzx.com

================================================================================
来源：http://aou.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://xti.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yco.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://byk.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://bsq.cheryme.top

TS:   JSON.stringify(obj)
来源：http://qpu.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kup.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://pgx.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://vus.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://hfp.xuanzx.com

[K02] JSON 字符串转对象
来源：http://oyn.guowangkeji.top

Py:   json.loads(s)
来源：http://ull.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tzo.hnqzz.top

JS:   JSON.parse(s)
来源：http://lsg.ehwqpu.com

TS:   JSON.parse(s)
来源：http://pgs.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xgv.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ray.redwolf501.top

Ruby: JSON.parse(s)
来源：http://jvu.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ind.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://uxt.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://acp.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://seh.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rue.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ohl.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uqm.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xdh.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://vwi.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vbo.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://dcw.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mqp.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ckp.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dqy.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://azc.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mtc.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lhe.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cev.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ikz.epnwcf.com

[K05] 深拷贝对象
来源：http://nve.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://zzs.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://odv.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://qnq.yj20258888.top

TS:   structuredClone(obj)
来源：http://vsd.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wgk.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sex.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hcb.pycfn.com

C#:   // 序列化往返，或自定义 Clone
来源：http://tmi.fengsongda.top

[K06] 解析 URL 查询串
来源：http://coz.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://btu.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ags.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lyp.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qtu.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jdv.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://frh.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://drj.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://foe.jinyuanbaomall.cn

[K07] 进制转换
来源：http://grm.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pio.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jgq.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://auj.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rxl.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kqc.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bhc.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vjh.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aaj.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://kus.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://qxb.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uvx.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://uqv.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://nyt.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pqa.shzxlz.cn

Go:   encoding/gob
来源：http://ynk.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://jpf.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tsb.pengpengdd.cyou

================================================================================
来源：http://idm.iojbl.cn

L. 网络请求
来源：http://dne.aibaodan.cn

================================================================================
来源：http://hkj.cqqwz.cn

[L01] 发送 GET 请求
来源：http://fju.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://upn.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rfi.mhx1999.top

JS:   await fetch(url)
来源：http://jyb.fengsongda.top

TS:   await fetch(url)
来源：http://qyn.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tit.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://exz.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://foo.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://huk.iojbl.cn

[L02] 发送 POST JSON
来源：http://odb.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ort.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mlu.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zzv.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kmr.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://plp.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mbz.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nad.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fvs.yvedp.cn

[L03] 设置自定义请求头
来源：http://whe.cdnleiting.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dxl.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nax.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxg.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fdk.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hqo.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dfb.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qir.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://luf.nanxuanxn.top

[L04] 设置超时
来源：http://qrj.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://izn.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yqh.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kfr.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdt.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://flx.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xko.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nit.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mii.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://lwd.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://khd.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nvu.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zki.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mmo.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jjn.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jnb.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nnk.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zad.cucudq.cn

[L06] 解析响应为 JSON
来源：http://dgk.feifeiyinyue.top

Py:   resp.json()
来源：http://ohw.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://adj.haohaochexian.top

JS:   await resp.json()
来源：http://mqz.yvedp.cn

TS:   await resp.json()
来源：http://fwh.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kjk.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jpa.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://gyr.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dcm.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://wzf.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bve.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ukc.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://umd.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://vog.fehbvm.com

Java: resp.statusCode()
来源：http://tzg.andypj.xyz

Go:   resp.StatusCode
来源：http://bvx.zhixingplan.top

Ruby: resp.code.to_i
来源：http://cmh.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://pqe.birdmap.top

[L08] 并发请求多个地址
来源：http://oyy.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eer.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://dqt.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxe.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vsx.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://twn.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xmj.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bca.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vlj.zycfv.cn

================================================================================
来源：http://amf.sweek.top

M. 命令行 / 进程 / 环境
来源：http://srm.hcnkem.com

================================================================================
来源：http://wyt.yuanzhike.top

[M01] 读取命令行参数
来源：http://fos.cashguo.top

Py:   sys.argv[1:]
来源：http://pit.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://zdv.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://aen.yongpay.top

TS:   process.argv.slice(2)
来源：http://rqf.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://ssv.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://lwh.zhaomingkeji.xyz

Ruby: ARGV
来源：http://zea.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://oyn.tarul.cn

[M02] 读取环境变量
来源：http://nay.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://xpx.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nnx.zhixingplan.top

JS:   process.env.HOME
来源：http://xdz.hammf.cn

TS:   process.env.HOME
来源：http://qhf.hywenlv.cn

Java: System.getenv("HOME")
来源：http://hxc.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wdv.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://dti.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sgu.jinqigufen.top

[M03] 执行外部命令
来源：http://myv.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://shq.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://idc.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sfq.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jiq.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kij.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ixe.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wth.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://ina.pycfn.com

[M04] 获取当前工作目录
来源：http://hqf.ctjpmb.com

Py:   os.getcwd()
来源：http://vgj.cqqwz.cn

PHP:  getcwd();
来源：http://jqg.jqgfzy.top

JS:   process.cwd()
来源：http://onn.c1oappe.top

TS:   process.cwd()
来源：http://gzt.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://hzb.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://wvq.yj202588.top

Ruby: Dir.pwd
来源：http://gsv.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://mpx.tarul.cn

[M05] 设置退出码
来源：http://mrj.yueranfly.top

Py:   sys.exit(1)
来源：http://aky.nanxinkj.top

PHP:  exit(1);
来源：http://goh.birdmap.top

JS:   process.exit(1)
来源：http://eba.cdnleiting.top

TS:   process.exit(1)
来源：http://ozu.zhengqikj.top

Java: System.exit(1)
来源：http://ark.sweek.top

Go:   os.Exit(1)
来源：http://wpr.quarkkingdee.top

Ruby: exit 1
来源：http://wxf.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gsk.52xcode.cn

[M06] 向标准错误输出
来源：http://pgl.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://ycz.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fjo.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://uda.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://zud.hnqzz.top

Java: System.err.println("err")
来源：http://nvz.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bmx.nwbrower.top

Ruby: warn "err"
来源：http://jqm.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://qar.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://nma.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://asa.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pmv.zycfv.cn

JS:   require.main === module
来源：http://wfc.sweek.top

TS:   require.main === module
来源：http://ukn.cheryme.top

Java: public static void main(String[] args)
来源：http://lxz.cqqwz.cn

Go:   func main()
来源：http://zjd.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nch.yonumen.top

C#:   static void Main(string[] args)
来源：http://tux.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://pkd.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://yol.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://fga.nanxinkj.top

JS:   process.platform;  process.version
来源：http://kuh.zdbjq.cn

TS:   process.platform;  process.version
来源：http://cos.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pmn.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mvq.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://grq.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://tpk.smart0.xyz

================================================================================
来源：http://qrr.bbcook.cn

N. 数据结构与算法
来源：http://pzh.xuanzx.com

================================================================================
来源：http://thi.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://ezr.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://xuu.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sde.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://roz.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://exj.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lbi.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://wlk.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xwt.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://qwm.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://prd.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://zbg.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yqm.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wmy.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://vdy.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nzm.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://gvo.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://nax.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pys.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://cwq.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lcz.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://haa.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dtf.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oxq.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cdb.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fku.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eez.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://gsk.hywenlv.cn

[N04] 斐波那契数列
来源：http://tyh.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iaw.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vxf.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozc.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://udb.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lcx.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eak.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bkv.ydjk.org.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uum.xziqi.cn

[N05] 最大公约数
来源：http://ygp.wangdashe.top

Py:   math.gcd(a, b)
来源：http://vyf.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fel.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqk.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yyb.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rta.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kmt.jiagoushi.top

Ruby: a.gcd(b)
来源：http://clj.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ovi.smart0.xyz

[N06] 判断回文字符串
来源：http://hle.chenlongwang.top

Py:   s == s[::-1]
来源：http://ojo.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://skr.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://trg.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://quj.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jlv.yfazqb.com

Go:   // 双指针从两端比较
来源：http://glg.bjfxy.top

Ruby: s == s.reverse
来源：http://pbm.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://afv.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://btr.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dde.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ptn.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hww.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://ahk.yj20258.top

Java: // 手写 HashMap
来源：http://rjh.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://kqi.jyoumei.cn

Ruby: // 手写 Hash
来源：http://fcn.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://syt.shuidangran.top

[N08] 生成全排列
来源：http://wto.zhijiandao.cn


<!-- 参考信息 -->