代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://bdl.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dcr.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nqb.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dxz.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pft.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ybh.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iqy.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jvw.birdmap.top

================================================================================
来源：http://ofm.hesvh.cn

K. JSON 与序列化
来源：http://dyu.9152youxi.cn

================================================================================
来源：http://xkw.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://lmc.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ryr.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bvr.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://liq.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://uig.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dgn.xziqi.cn

Go:   json.Marshal(obj)
来源：http://kuj.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hfn.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://drc.nwbrower.top

[K02] JSON 字符串转对象
来源：http://qzx.nanxuanxn.top

Py:   json.loads(s)
来源：http://zsm.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bdr.pycfn.com

JS:   JSON.parse(s)
来源：http://wpn.redwolf501.top

TS:   JSON.parse(s)
来源：http://pyq.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rrz.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://yqq.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://lzw.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://awx.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://tod.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://raw.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://twl.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aqb.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nan.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wgd.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xbt.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ukl.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://shv.yj20258.top

[K04] 读取 JSON 文件
来源：http://wbo.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vxc.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mjd.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pia.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rwx.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rua.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hqv.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wbw.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jxh.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://gmx.sweek.top

Py:   copy.deepcopy(obj)
来源：http://ciy.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://wqr.zdqjudy.top

JS:   structuredClone(obj)
来源：http://zsg.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://btx.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://srb.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hhp.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cwg.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gql.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://afk.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://foc.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ehv.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zwq.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://onq.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jfs.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tvd.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wnq.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zdf.shanyushiyangtech.top

[K07] 进制转换
来源：http://piz.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ddc.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sjg.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wuc.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pmt.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cqm.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://els.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://efm.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hky.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://zwa.yongpay.top

Py:   pickle.dumps(obj)
来源：http://cvg.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qyr.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://rwk.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://btz.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tlg.ehwqpu.com

Go:   encoding/gob
来源：http://nem.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://ywy.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gox.zdbjq.cn

================================================================================
来源：http://sqz.ivvv.top

L. 网络请求
来源：http://snl.yanxiufei.cn

================================================================================
来源：http://hjl.cashguo.top

[L01] 发送 GET 请求
来源：http://fio.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://umo.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://diy.zycfv.cn

JS:   await fetch(url)
来源：http://mhy.52xcode.cn

TS:   await fetch(url)
来源：http://wbh.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ylb.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://vck.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sgf.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://khk.haohaochexian.top

[L02] 发送 POST JSON
来源：http://rjq.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vbm.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qrb.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kom.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pfp.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jtx.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vkf.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wqc.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ytb.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://rfk.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://szd.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cms.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nax.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dfb.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gxr.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://myg.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vnj.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ldm.ywan-chungtsiang.top

[L04] 设置超时
来源：http://gfl.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://glx.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fcy.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxw.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yqq.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mrp.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hcs.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qlo.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vha.52xcode.cn

[L05] 上传文件（multipart）
来源：http://nyr.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://shj.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kja.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cpp.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://adt.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qpw.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ioe.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://asy.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jdv.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://wib.sysykeji.top

Py:   resp.json()
来源：http://obh.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://lud.daria6918.cn

JS:   await resp.json()
来源：http://tqh.jianghu66.top

TS:   await resp.json()
来源：http://cmt.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://swy.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://avs.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://peq.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ued.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://plc.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://afz.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kpi.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://mwj.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://gkh.cashguo.top

Java: resp.statusCode()
来源：http://bfv.shzxlz.cn

Go:   resp.StatusCode
来源：http://itm.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://jul.hammf.cn

C#:   (int)resp.StatusCode
来源：http://mjd.gzhubu.top

[L08] 并发请求多个地址
来源：http://axp.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nur.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://daw.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdo.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mdx.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://san.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kgc.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ucw.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lph.c1oappe.top

================================================================================
来源：http://isy.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://pst.guannengcc.top

================================================================================
来源：http://tkk.zycfv.cn

[M01] 读取命令行参数
来源：http://vkt.andypj.xyz

Py:   sys.argv[1:]
来源：http://xet.316326.xyz

PHP:  $argv;  $argc;
来源：http://bmr.tanke756.top

JS:   process.argv.slice(2)
来源：http://ust.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://msf.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://uru.hnqzz.top

Go:   os.Args[1:]
来源：http://hgm.xziqi.cn

Ruby: ARGV
来源：http://adj.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://wei.sysykeji.top

[M02] 读取环境变量
来源：http://aik.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://bgj.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gcn.hnxiangtu.top

JS:   process.env.HOME
来源：http://oyh.hnqzz.top

TS:   process.env.HOME
来源：http://byg.jiagoushi.top

Java: System.getenv("HOME")
来源：http://ahl.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oyy.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://afq.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lnz.xuetiantiany.cn

[M03] 执行外部命令
来源：http://xzb.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ads.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hnl.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mhm.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bsc.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wec.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://apo.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://rjr.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://fkt.fengsongda.top

[M04] 获取当前工作目录
来源：http://owh.gzhubu.top

Py:   os.getcwd()
来源：http://gqm.xinyue.icu

PHP:  getcwd();
来源：http://fqn.gotoacloud.top

JS:   process.cwd()
来源：http://rjd.jyoumei.cn

TS:   process.cwd()
来源：http://xsw.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://goi.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://ane.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://syl.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gaj.zhoulong.xyz

[M05] 设置退出码
来源：http://roo.haohaochexian.top

Py:   sys.exit(1)
来源：http://rya.chenlongwang.top

PHP:  exit(1);
来源：http://fxr.vqdsnc.cn

JS:   process.exit(1)
来源：http://psj.havefunace.top

TS:   process.exit(1)
来源：http://vyq.wangdashe.top

Java: System.exit(1)
来源：http://osv.yanxiufei.cn

Go:   os.Exit(1)
来源：http://xlz.quarkkingdee.top

Ruby: exit 1
来源：http://rib.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gzi.epnwcf.com

[M06] 向标准错误输出
来源：http://ryw.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://ptd.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://btx.sxryk.cn

JS:   console.error("err")
来源：http://oeq.sufxvd.cn

TS:   console.error("err")
来源：http://umt.zhoulong.xyz

Java: System.err.println("err")
来源：http://rnw.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aey.hongshengwenyu.top

Ruby: warn "err"
来源：http://vya.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://vvc.aizwys.cn

[M07] 判断是否为主入口
来源：http://kwd.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://bcy.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jfd.sweek.top

JS:   require.main === module
来源：http://ctv.jinyuanbaomall.cn

TS:   require.main === module
来源：http://cai.iojbl.cn

Java: public static void main(String[] args)
来源：http://zcu.shzxlz.cn

Go:   func main()
来源：http://iuz.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://epp.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://emr.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://sxu.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://csp.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://kfa.meibo888.top

JS:   process.platform;  process.version
来源：http://ftf.yongpay.top

TS:   process.platform;  process.version
来源：http://ywk.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhz.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://odj.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mps.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ejj.svipenyu.cn

================================================================================
来源：http://qai.hywenlv.cn

N. 数据结构与算法
来源：http://xxd.hnqzz.top

================================================================================
来源：http://rvx.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://kei.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://kqs.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mxb.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yng.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snt.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://npg.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://wpv.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://piz.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uci.fzhhl.top

[N02] 排序（工程实践用内置实现）
来源：http://kpe.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://iew.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uab.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fay.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://spy.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sxu.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://sze.tarul.cn

Ruby: arr.sort
来源：http://uql.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://cjc.yongpay.top

[N03] 快速排序（分治示例）
来源：http://kgt.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mkg.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://xxn.9152youxi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oat.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aen.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ubu.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pax.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mbv.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://cmf.tianlin.xyz

[N04] 斐波那契数列
来源：http://oku.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://idd.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://prh.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gcy.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zoz.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ioe.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eid.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fzv.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bea.tian-w.cn

[N05] 最大公约数
来源：http://gxe.hcnkem.com

Py:   math.gcd(a, b)
来源：http://die.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qep.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://knh.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xvj.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uvp.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eth.sxryk.cn

Ruby: a.gcd(b)
来源：http://yhz.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jbf.bjfxy.top

[N06] 判断回文字符串
来源：http://twx.yonumen.top

Py:   s == s[::-1]
来源：http://jrb.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://vgo.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://vkd.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://yay.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jfs.c1oappe.top

Go:   // 双指针从两端比较
来源：http://gig.daria6918.cn

Ruby: s == s.reverse
来源：http://vyw.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dzd.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://gde.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ppj.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pdu.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vdd.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://lpe.ehwqpu.com

Java: // 手写 HashMap
来源：http://xwb.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://lvc.guowangkeji.top

Ruby: // 手写 Hash
来源：http://rka.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://pyu.yanxiufei.cn

[N08] 生成全排列
来源：http://cfb.gzhubu.top


<!-- 参考信息 -->