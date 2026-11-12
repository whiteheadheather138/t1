代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hyu.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cci.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ywh.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://esq.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://esa.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ylr.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xth.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eok.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gia.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kxh.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vyr.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://niq.fanxiaobao.xyz

================================================================================
来源：http://twm.ehwqpu.com

K. JSON 与序列化
来源：http://las.yj20258.top

================================================================================
来源：http://yug.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://bly.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uie.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ull.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://rtw.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://neb.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sxz.shuidangran.top

Go:   json.Marshal(obj)
来源：http://xnn.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://roy.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fji.hnqzz.top

[K02] JSON 字符串转对象
来源：http://txp.zhiwuduotai.top

Py:   json.loads(s)
来源：http://koy.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mdt.jinqigufen.top

JS:   JSON.parse(s)
来源：http://bhc.hammf.cn

TS:   JSON.parse(s)
来源：http://fpj.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pce.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://yiw.havefunace.top

Ruby: JSON.parse(s)
来源：http://stj.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jgb.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://yik.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mzu.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mfk.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qcw.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zpb.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ine.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wtl.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bve.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gxl.yonumen.top

[K04] 读取 JSON 文件
来源：http://gpn.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eab.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://igu.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dne.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rzl.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aij.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zfb.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ifb.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dyu.bjfxy.top

[K05] 深拷贝对象
来源：http://nzx.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://igr.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://nne.shuidangran.top

JS:   structuredClone(obj)
来源：http://kkj.bjfxy.top

TS:   structuredClone(obj)
来源：http://xnu.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bkv.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://okn.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kwk.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jcz.zhiwuduotai.top

[K06] 解析 URL 查询串
来源：http://afv.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fko.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://llr.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agn.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dgj.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nfg.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kxg.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jyr.daxiang520.top

[K07] 进制转换
来源：http://znc.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qid.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fmm.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fmj.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jrc.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://svh.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jtd.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ybg.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://obr.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://wkv.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://fdi.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ftn.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://htd.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://hpr.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fbs.cucudq.cn

Go:   encoding/gob
来源：http://ksx.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://fcf.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fbe.gaohongyu789.top

================================================================================
来源：http://fes.cucudq.cn

L. 网络请求
来源：http://aqd.yvedp.cn

================================================================================
来源：http://iqs.ctjpmb.com

[L01] 发送 GET 请求
来源：http://gbk.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nbj.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://acw.yueranfly.top

JS:   await fetch(url)
来源：http://emc.hesvh.cn

TS:   await fetch(url)
来源：http://fir.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://adn.sweek.top

Go:   resp, err := http.Get(url)
来源：http://bei.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cot.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kdc.hammf.cn

[L02] 发送 POST JSON
来源：http://dsc.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bok.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jyb.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lsn.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fdp.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nac.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://psv.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nyh.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rex.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://kkr.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uos.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vzk.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tui.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ywr.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sft.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jhg.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pam.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sfm.gaohongyu789.top

[L04] 设置超时
来源：http://qvj.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://jvv.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fgu.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zle.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mnu.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ylu.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sou.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mrg.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mmm.cucudq.cn

[L05] 上传文件（multipart）
来源：http://uzd.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bqb.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fuc.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ehv.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://boe.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mcb.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://euj.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nws.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gtw.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://apa.mhx1999.top

Py:   resp.json()
来源：http://xms.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://lol.yangfankeji.com

JS:   await resp.json()
来源：http://yhu.gotoacloud.top

TS:   await resp.json()
来源：http://kjz.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ihx.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vvo.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://zmd.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://loi.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://kjq.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dbg.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fzr.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://ckx.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://hvg.yuanzhike.top

Java: resp.statusCode()
来源：http://pea.pycfn.com

Go:   resp.StatusCode
来源：http://nhy.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://snk.tarul.cn

C#:   (int)resp.StatusCode
来源：http://bwa.yvedp.cn

[L08] 并发请求多个地址
来源：http://qfp.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tgc.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://kth.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hqb.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uac.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://edh.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xhw.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fcv.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dcp.fktsv.cn

================================================================================
来源：http://uvb.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://eby.yuanzhike.top

================================================================================
来源：http://qrl.fengsongda.top

[M01] 读取命令行参数
来源：http://gzf.aibaodan.cn

Py:   sys.argv[1:]
来源：http://yvl.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://rks.52xcode.cn

JS:   process.argv.slice(2)
来源：http://wiq.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://ceu.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://aab.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://ugk.tarul.cn

Ruby: ARGV
来源：http://yss.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://glq.hnxiangtu.top

[M02] 读取环境变量
来源：http://jfm.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://vyc.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sst.dashuyun.cn

JS:   process.env.HOME
来源：http://qcm.yj202588.top

TS:   process.env.HOME
来源：http://kub.sweek.top

Java: System.getenv("HOME")
来源：http://wdg.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xda.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://ybz.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fuv.yvedp.cn

[M03] 执行外部命令
来源：http://giy.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pgp.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pqg.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bsd.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://usg.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lbu.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://zbm.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://oxp.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://eot.gotoacloud.top

[M04] 获取当前工作目录
来源：http://knw.hywenlv.cn

Py:   os.getcwd()
来源：http://mqu.tarul.cn

PHP:  getcwd();
来源：http://gmt.zdbjq.cn

JS:   process.cwd()
来源：http://bvv.chenzaomai.com

TS:   process.cwd()
来源：http://dux.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://axf.vehdjk.com

Go:   os.Getwd()
来源：http://dyf.xuanzx.com

Ruby: Dir.pwd
来源：http://aiy.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xbr.cheryme.top

[M05] 设置退出码
来源：http://qpd.nanxinkj.top

Py:   sys.exit(1)
来源：http://qmx.xinyue.icu

PHP:  exit(1);
来源：http://rsc.hfpthk.cn

JS:   process.exit(1)
来源：http://idc.52xcode.cn

TS:   process.exit(1)
来源：http://ckp.jqgufenzy.top

Java: System.exit(1)
来源：http://ihd.dashuyun.cn

Go:   os.Exit(1)
来源：http://ytm.zhoulong.xyz

Ruby: exit 1
来源：http://gny.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://amg.cdnleiting.top

[M06] 向标准错误输出
来源：http://mfy.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://rzr.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://juv.c1oappe.top

JS:   console.error("err")
来源：http://fut.jyoumei.cn

TS:   console.error("err")
来源：http://nai.ydzc1.top

Java: System.err.println("err")
来源：http://ezh.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wmn.tianlin.xyz

Ruby: warn "err"
来源：http://wag.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://awr.9152youxi.cn

[M07] 判断是否为主入口
来源：http://woy.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://gvh.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ito.yuanzhike.top

JS:   require.main === module
来源：http://dgr.vqdsnc.cn

TS:   require.main === module
来源：http://hhp.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://zku.jiagoushi.top

Go:   func main()
来源：http://vhl.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rje.sxryk.cn

C#:   static void Main(string[] args)
来源：http://blu.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://dxd.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://yqb.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://vce.daxiang520.top

JS:   process.platform;  process.version
来源：http://rre.snrcjt.cn

TS:   process.platform;  process.version
来源：http://oqz.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ykc.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nhd.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ked.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://drc.fehbvm.com

================================================================================
来源：http://csh.jinqigufen.top

N. 数据结构与算法
来源：http://qjr.yj202588.top

================================================================================
来源：http://vkq.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://haa.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://hqj.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nmg.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ruz.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mvd.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://nop.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://sth.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hgr.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://qux.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://vnc.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://oqg.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nsv.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://war.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bzq.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vle.havefunace.top

Go:   slices.Sort(arr)
来源：http://say.zycfv.cn

Ruby: arr.sort
来源：http://pqf.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://hvg.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://vcp.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://idq.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://ctm.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lqw.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sgi.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nfn.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tok.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ovk.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://crz.xinyue.icu

[N04] 斐波那契数列
来源：http://kma.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mrc.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wgc.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mtt.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://frx.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ezk.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dev.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oyw.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cyc.aizwys.cn

[N05] 最大公约数
来源：http://vlq.havefunace.top

Py:   math.gcd(a, b)
来源：http://qyy.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hgb.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rel.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgl.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tsc.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cpq.redwolf501.top

Ruby: a.gcd(b)
来源：http://jpt.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jcw.zhongyouzk.top

[N06] 判断回文字符串
来源：http://upl.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://iqc.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://gho.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://zqm.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://tkq.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vxn.andypj.xyz

Go:   // 双指针从两端比较
来源：http://vqi.daria6918.cn

Ruby: s == s.reverse
来源：http://nbj.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://whg.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://nfi.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hts.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pdp.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cmp.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://mfx.cheryme.top

Java: // 手写 HashMap
来源：http://azb.cashguo.top


<!-- 参考信息 -->