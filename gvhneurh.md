代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://fur.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xep.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bwe.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://enk.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ewa.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zfc.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://umk.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lpg.guannengcc.top

================================================================================
来源：http://uqs.tianlin.xyz

K. JSON 与序列化
来源：http://kij.fktsv.cn

================================================================================
来源：http://hak.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://ffn.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zpm.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hem.pycfn.com

JS:   JSON.stringify(obj)
来源：http://dve.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://cnn.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://osq.redwolf501.top

Go:   json.Marshal(obj)
来源：http://pkc.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://bau.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://vgq.hesvh.cn

[K02] JSON 字符串转对象
来源：http://xnf.wangshuangyany.cn

Py:   json.loads(s)
来源：http://weq.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yps.mhx1999.top

JS:   JSON.parse(s)
来源：http://qzh.yuanzhike.top

TS:   JSON.parse(s)
来源：http://pth.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ark.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://ahz.yj20258888.top

Ruby: JSON.parse(s)
来源：http://bei.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tvf.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://cti.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sqm.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dff.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pyc.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rru.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jqu.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hxd.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://rgz.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qcj.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://avx.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://awf.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nvi.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bii.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pza.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://law.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cqm.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cph.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qba.xziqi.cn

[K05] 深拷贝对象
来源：http://ari.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://ofz.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://pjk.9152youxi.cn

JS:   structuredClone(obj)
来源：http://kok.yj202588.top

TS:   structuredClone(obj)
来源：http://dxy.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nha.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gpa.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hax.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://avy.aizwys.cn

[K06] 解析 URL 查询串
来源：http://rnp.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wno.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hxm.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zlr.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ayg.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xhx.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xuo.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yxd.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nbw.mhx1999.top

[K07] 进制转换
来源：http://fqv.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xiz.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jac.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ecu.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mnq.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kph.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vez.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yed.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dvi.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://heg.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://xkz.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://syc.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://zwk.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://xng.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://umz.zhoulong.xyz

Go:   encoding/gob
来源：http://xtx.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://zxj.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dnw.xylfe.cn

================================================================================
来源：http://dvv.shanyushiyangtech.top

L. 网络请求
来源：http://lpr.9152youxi.cn

================================================================================
来源：http://hqk.smart0.xyz

[L01] 发送 GET 请求
来源：http://ort.jinqigfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zaw.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jnf.9152youxi.cn

JS:   await fetch(url)
来源：http://xbc.hnqzz.top

TS:   await fetch(url)
来源：http://jfw.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ezz.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://uih.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://sin.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ezg.aizwys.cn

[L02] 发送 POST JSON
来源：http://qoy.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://xyf.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lby.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rvb.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qdr.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kbl.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ent.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sua.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ppp.epnwcf.com

[L03] 设置自定义请求头
来源：http://ifq.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dzl.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mzf.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fri.dashuyun.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zon.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vuk.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nrz.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ozf.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wjl.jyoumei.cn

[L04] 设置超时
来源：http://edq.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://jwh.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dvv.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzh.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jmp.feifeiyinyue.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kgo.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rxr.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://com.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://drd.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://kqx.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zym.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tsd.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ttr.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tbd.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fns.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sxc.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pas.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eig.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://dpd.sweek.top

Py:   resp.json()
来源：http://bmn.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://nhf.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://itr.uphjek.com

TS:   await resp.json()
来源：http://yxw.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aif.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gsb.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://zcy.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rcw.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://aar.sjlbkw.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bdr.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qke.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://edm.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://dpm.fzhhl.top

Java: resp.statusCode()
来源：http://yzj.fzhhl.top

Go:   resp.StatusCode
来源：http://hzy.snrcjt.cn

Ruby: resp.code.to_i
来源：http://uyv.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://zlj.xziqi.cn

[L08] 并发请求多个地址
来源：http://luq.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pbz.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://ing.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzq.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mwn.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iad.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fwh.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lti.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oal.yj20258.top

================================================================================
来源：http://rnr.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://bcs.hesvh.cn

================================================================================
来源：http://tdz.haohaochexian.top

[M01] 读取命令行参数
来源：http://vba.guannengcc.top

Py:   sys.argv[1:]
来源：http://yvt.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://llp.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://hfs.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://oxa.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://knp.cashguo.top

Go:   os.Args[1:]
来源：http://pmb.shanyushiyangtech.top

Ruby: ARGV
来源：http://dvm.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://kwd.havefunace.top

[M02] 读取环境变量
来源：http://zqz.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://ipv.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yhi.wangdashe.top

JS:   process.env.HOME
来源：http://bqh.yanxiufei.cn

TS:   process.env.HOME
来源：http://xwn.yangfankeji.com

Java: System.getenv("HOME")
来源：http://lrb.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jnd.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://bou.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bcc.havefunace.top

[M03] 执行外部命令
来源：http://oso.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rxb.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xrz.hysaishi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://way.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ntm.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gnv.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kjs.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://ddk.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://bzp.yangfankeji.com

[M04] 获取当前工作目录
来源：http://ctx.xuanzx.com

Py:   os.getcwd()
来源：http://mwl.havefunace.top

PHP:  getcwd();
来源：http://xdv.iojbl.cn

JS:   process.cwd()
来源：http://hwu.nanxuanxn.top

TS:   process.cwd()
来源：http://uzy.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://kth.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://fct.nanxinkj.top

Ruby: Dir.pwd
来源：http://qfs.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wxy.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://xar.jqgufenzy.top

Py:   sys.exit(1)
来源：http://ncp.havefunace.top

PHP:  exit(1);
来源：http://fis.smart0.xyz

JS:   process.exit(1)
来源：http://ght.redwolf501.top

TS:   process.exit(1)
来源：http://nji.zdbjq.cn

Java: System.exit(1)
来源：http://ijn.jinqigufen.top

Go:   os.Exit(1)
来源：http://xfj.zhiwuduotai.top

Ruby: exit 1
来源：http://rlw.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sns.bbcook.cn

[M06] 向标准错误输出
来源：http://ayt.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://ojh.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vgh.cucudq.cn

JS:   console.error("err")
来源：http://unb.gotoacloud.top

TS:   console.error("err")
来源：http://eja.haohaochexian.top

Java: System.err.println("err")
来源：http://lhm.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ote.cashguo.top

Ruby: warn "err"
来源：http://rvn.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ovu.birdmap.top

[M07] 判断是否为主入口
来源：http://prd.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://kkb.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qgn.zdbjq.cn

JS:   require.main === module
来源：http://xul.cheryme.top

TS:   require.main === module
来源：http://itd.yonumen.top

Java: public static void main(String[] args)
来源：http://vuo.yongpay.top

Go:   func main()
来源：http://ewh.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qkm.fengsongda.top

C#:   static void Main(string[] args)
来源：http://bma.cashguo.top

[M08] 获取系统与运行时信息
来源：http://dut.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://vzt.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://gmz.mhx1999.top

JS:   process.platform;  process.version
来源：http://glt.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://lin.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yjk.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://izd.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jdf.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ohf.yuxming.cn

================================================================================
来源：http://djj.redwolf501.top

N. 数据结构与算法
来源：http://mmi.jinqigfzy.top

================================================================================
来源：http://cap.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://dgg.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qpo.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://etz.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bqe.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gwl.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://ylu.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://cgn.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jag.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://xcf.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://cea.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://qbr.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://snv.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jzf.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lnm.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pcs.bjfxy.top

Go:   slices.Sort(arr)
来源：http://vng.ivvv.top

Ruby: arr.sort
来源：http://woq.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://tsw.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://viw.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pyc.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://str.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dfe.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ueh.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sut.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://puk.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ysh.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zqe.yj202588.top

[N04] 斐波那契数列
来源：http://snx.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ztd.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thr.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yjx.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvb.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://buk.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bgx.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fcd.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nkp.gzhubu.top

[N05] 最大公约数
来源：http://lyx.fzhhl.top

Py:   math.gcd(a, b)
来源：http://cvp.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mcs.svipenyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cmz.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wek.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gba.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pbr.yongpay.top

Ruby: a.gcd(b)
来源：http://njn.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qdr.tanke756.top

[N06] 判断回文字符串
来源：http://azq.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://jed.shuidangran.top

PHP:  $s === strrev($s);
来源：http://gvv.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://hkx.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://jaf.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sag.daxiang520.top

Go:   // 双指针从两端比较
来源：http://ghs.jiagoushi.top

Ruby: s == s.reverse
来源：http://ihv.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kls.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://zor.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rlk.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qgv.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://feb.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://dez.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://hdx.yvedp.cn

Go:   // 手写 map[int]int
来源：http://xxp.zycfv.cn

Ruby: // 手写 Hash
来源：http://wwj.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hoh.jlsjyb.cn

[N08] 生成全排列
来源：http://nor.sysykeji.top


<!-- 参考信息 -->