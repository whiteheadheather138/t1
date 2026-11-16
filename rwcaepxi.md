代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://fmd.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kqh.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uml.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bdh.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jxb.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wur.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qgo.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cai.zhixingplan.top

================================================================================
来源：http://rrg.hnqzz.top

K. JSON 与序列化
来源：http://fri.aibaodan.cn

================================================================================
来源：http://eua.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://ywf.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wzh.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lwo.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://aik.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://ibe.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://noc.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://enm.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://emd.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fjv.52xcode.cn

[K02] JSON 字符串转对象
来源：http://wkl.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://gfk.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://srk.tanke756.top

JS:   JSON.parse(s)
来源：http://cno.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://zpv.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aqw.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://qcw.sysykeji.top

Ruby: JSON.parse(s)
来源：http://drf.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vhn.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://uwh.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xia.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qsn.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xko.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://trp.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nxu.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://esj.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ura.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://whk.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://tas.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jkk.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eli.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scm.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://foe.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bzv.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://spl.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ahu.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lbn.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://eqn.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://xst.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://ilb.jinqigufen.top

JS:   structuredClone(obj)
来源：http://udw.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://mwh.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bzl.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hlm.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ckb.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ase.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://scn.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qyv.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bkg.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wqb.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ybs.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://arl.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://dhq.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zom.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gnc.zdqjudy.top

[K07] 进制转换
来源：http://lpq.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lon.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zxf.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xqn.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rmi.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://obo.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nqa.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hci.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rrv.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://alk.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://buf.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yig.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://gmz.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://iam.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jvn.feifeiyinyue.top

Go:   encoding/gob
来源：http://knr.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://tya.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lkl.nanxuanxn.top

================================================================================
来源：http://mqm.jinghuilouyu.cn

L. 网络请求
来源：http://qhu.zdqjudy.top

================================================================================
来源：http://aek.chenlongwang.top

[L01] 发送 GET 请求
来源：http://gms.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qys.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zzt.jqgufenzy.top

JS:   await fetch(url)
来源：http://axw.nanxuanxn.top

TS:   await fetch(url)
来源：http://qpb.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qst.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://pji.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://zmz.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jzv.hnqzz.top

[L02] 发送 POST JSON
来源：http://etx.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kig.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kjf.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://flf.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://efq.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ber.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mha.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wte.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xqc.redwolf501.top

[L03] 设置自定义请求头
来源：http://yjn.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ogy.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bjz.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tmb.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnp.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ykx.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uwy.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zmn.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uwv.zdqjudy.top

[L04] 设置超时
来源：http://kxu.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://qja.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qfq.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lgn.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://teq.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kgo.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ljf.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://awi.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ybo.iojbl.cn

[L05] 上传文件（multipart）
来源：http://stn.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nxu.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ojn.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cff.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tuq.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qkn.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lcx.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vto.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vpn.yfazqb.com

[L06] 解析响应为 JSON
来源：http://mqd.mhx1999.top

Py:   resp.json()
来源：http://mvd.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://spv.jiagoushi.top

JS:   await resp.json()
来源：http://jex.feifeiyinyue.top

TS:   await resp.json()
来源：http://xwk.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vhb.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://whh.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://tcs.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fcd.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://hpv.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lnv.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tpp.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://dwl.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://mbi.vehdjk.com

Java: resp.statusCode()
来源：http://rvx.ybcxt.top

Go:   resp.StatusCode
来源：http://lsu.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://rtg.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://dri.gotoacloud.top

[L08] 并发请求多个地址
来源：http://aga.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eyd.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://ruf.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kmw.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bmk.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eyf.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fhe.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jsq.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qzx.yangfankeji.com

================================================================================
来源：http://ymi.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://ijq.shanyushiyangtech.top

================================================================================
来源：http://owj.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://dnh.xylfe.cn

Py:   sys.argv[1:]
来源：http://zam.xinyue.icu

PHP:  $argv;  $argc;
来源：http://bjg.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://tdx.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://ewk.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://qth.9152youxi.cn

Go:   os.Args[1:]
来源：http://gch.chenlongwang.top

Ruby: ARGV
来源：http://lba.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://mul.chenjidiqi.icu

[M02] 读取环境变量
来源：http://uem.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://pdd.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sbu.zhijiandao.cn

JS:   process.env.HOME
来源：http://joo.chenzaomai.com

TS:   process.env.HOME
来源：http://ecv.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://tzo.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xaw.iojbl.cn

Ruby: ENV["HOME"]
来源：http://xpn.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bqr.yvedp.cn

[M03] 执行外部命令
来源：http://jvy.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ely.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cmk.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uyn.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tyc.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zpn.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rvk.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://qfe.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://xnx.ybcxt.top

[M04] 获取当前工作目录
来源：http://oop.epnwcf.com

Py:   os.getcwd()
来源：http://mag.pycfn.com

PHP:  getcwd();
来源：http://qjx.hywenlv.cn

JS:   process.cwd()
来源：http://qlf.yongpay.top

TS:   process.cwd()
来源：http://pfd.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://kwh.hcnkem.com

Go:   os.Getwd()
来源：http://idx.ehwqpu.com

Ruby: Dir.pwd
来源：http://edp.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ddm.yuanzhike.top

[M05] 设置退出码
来源：http://bfu.hcnkem.com

Py:   sys.exit(1)
来源：http://cum.dianchejie.cn

PHP:  exit(1);
来源：http://fbw.ivvv.top

JS:   process.exit(1)
来源：http://nyc.epnwcf.com

TS:   process.exit(1)
来源：http://uhy.dashuyun.cn

Java: System.exit(1)
来源：http://flf.cucudq.cn

Go:   os.Exit(1)
来源：http://iqy.vqdsnc.cn

Ruby: exit 1
来源：http://tei.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yzw.jlsjyb.cn

[M06] 向标准错误输出
来源：http://otr.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://hjj.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cjn.xuanzx.com

JS:   console.error("err")
来源：http://bhg.ydzc1.top

TS:   console.error("err")
来源：http://nsu.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://mlc.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pvf.chenzaomai.com

Ruby: warn "err"
来源：http://khh.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://zwa.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://nzr.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://bpn.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dps.zycfv.cn

JS:   require.main === module
来源：http://wvi.sysykeji.top

TS:   require.main === module
来源：http://zfy.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://nfo.hnqzz.top

Go:   func main()
来源：http://ahd.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nwk.redwolf501.top

C#:   static void Main(string[] args)
来源：http://jcy.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://jvw.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://dxr.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://nlk.bbcook.cn

JS:   process.platform;  process.version
来源：http://lhc.sxryk.cn

TS:   process.platform;  process.version
来源：http://clo.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sdd.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://ruc.chenlongwang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mce.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wbk.vehdjk.com

================================================================================
来源：http://fhf.zdqjudy.top

N. 数据结构与算法
来源：http://faz.aizwys.cn

================================================================================
来源：http://jcb.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://vlq.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rlg.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nso.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vot.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xqo.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eyx.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://vgv.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rit.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://hjg.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://kcy.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vyg.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dfd.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eyo.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tzg.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hcz.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://gfz.hnqzz.top

Ruby: arr.sort
来源：http://qay.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xbd.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://okt.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://edl.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://zzh.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vce.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtf.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tfq.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dxb.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://quj.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://fvj.mhx1999.top

[N04] 斐波那契数列
来源：http://lek.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eku.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hzt.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyx.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nli.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nlo.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hfb.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dzg.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rdh.fzhhl.top

[N05] 最大公约数
来源：http://tko.mhx1999.top

Py:   math.gcd(a, b)
来源：http://cnz.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nym.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oku.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqx.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://btl.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iui.dashuyun.cn

Ruby: a.gcd(b)
来源：http://mxp.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fgh.xingfuxueyuan.xyz

[N06] 判断回文字符串
来源：http://wpi.zdbjq.cn

Py:   s == s[::-1]
来源：http://ema.bbcook.cn

PHP:  $s === strrev($s);
来源：http://lui.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://xiu.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://cca.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wps.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://qsm.sjlbkw.cn

Ruby: s == s.reverse
来源：http://gdt.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gjb.birdmap.top

[N07] 两数之和（返回下标）
来源：http://uxy.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ewb.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://epp.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mqz.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://fzh.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://pqp.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://ryk.ydzc1.top

Ruby: // 手写 Hash
来源：http://xjn.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jzm.jiagoushi.top

[N08] 生成全排列
来源：http://wkt.bjfxy.top


<!-- 参考信息 -->