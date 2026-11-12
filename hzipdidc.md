代发 wailian999

================================================================================
来源：http://dlr.fktsv.cn

K. JSON 与序列化
来源：http://thu.zhengqikj.top

================================================================================
来源：http://omm.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://jky.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ebu.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wad.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://pjy.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://hxw.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://boo.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://kzf.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wkb.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://tto.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://jfw.jianghu66.top

Py:   json.loads(s)
来源：http://ayz.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://teg.yj20258.top

JS:   JSON.parse(s)
来源：http://ypa.yj202588.top

TS:   JSON.parse(s)
来源：http://bmf.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uok.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://qth.pycfn.com

Ruby: JSON.parse(s)
来源：http://xdb.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lul.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://vzc.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hil.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hun.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://byf.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wcq.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ruq.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://znt.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://zmj.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mcw.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://eet.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ydr.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eju.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jlg.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ovq.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jbf.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kxp.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pbe.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vym.mhx1999.top

[K05] 深拷贝对象
来源：http://qiq.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://did.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://eqa.jqgfzy.top

JS:   structuredClone(obj)
来源：http://swt.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://deu.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ilx.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gjg.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ngg.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ohp.daria6918.cn

[K06] 解析 URL 查询串
来源：http://tkt.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vbj.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vks.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jfx.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aqh.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bfx.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ejm.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zsg.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ylz.9152youxi.cn

[K07] 进制转换
来源：http://nkj.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://doz.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ifx.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://trk.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pub.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kqu.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://phh.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wiq.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ikc.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://uzd.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://oom.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fau.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://ldo.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://yay.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wne.yuxming.cn

Go:   encoding/gob
来源：http://qvk.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://wly.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pff.hfpthk.cn

================================================================================
来源：http://lsi.zhaomingkeji.xyz

L. 网络请求
来源：http://wwq.nwbrower.top

================================================================================
来源：http://rbk.snrcjt.cn

[L01] 发送 GET 请求
来源：http://wrc.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ceg.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qph.svipenyu.cn

JS:   await fetch(url)
来源：http://mcv.yfazqb.com

TS:   await fetch(url)
来源：http://eek.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gnz.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://chw.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://vyn.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zrl.ppjwa.cn

[L02] 发送 POST JSON
来源：http://yus.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://xga.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gpc.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nun.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mzt.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gqd.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bme.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yvl.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dry.xziqi.cn

[L03] 设置自定义请求头
来源：http://gpo.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mau.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mzq.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dgz.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://esl.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pkv.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xoy.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tmo.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nar.sysykeji.top

[L04] 设置超时
来源：http://vpj.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://rua.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mtv.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wui.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vmd.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rnp.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yaw.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://muv.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gcl.tian-w.cn

[L05] 上传文件（multipart）
来源：http://xut.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xbl.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yqh.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uia.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://caa.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wbv.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vne.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sfr.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fza.birdmap.top

[L06] 解析响应为 JSON
来源：http://wea.nanxinkj.top

Py:   resp.json()
来源：http://kav.hnqzz.top

PHP:  json_decode($body, true);
来源：http://jao.aizwys.cn

JS:   await resp.json()
来源：http://mke.aibaodan.cn

TS:   await resp.json()
来源：http://kuc.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://okt.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://epx.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://feb.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nqv.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://mlk.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mzo.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cgg.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://ass.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://cbm.nanxuanxn.top

Java: resp.statusCode()
来源：http://zqo.sweek.top

Go:   resp.StatusCode
来源：http://ugb.sweek.top

Ruby: resp.code.to_i
来源：http://oha.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://zbx.shuidangran.top

[L08] 并发请求多个地址
来源：http://wox.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gha.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://emr.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lyx.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nll.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yhl.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ylg.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bdr.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://atv.hcnkem.com

================================================================================
来源：http://wlj.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://ecl.cheryme.top

================================================================================
来源：http://cnh.vehdjk.com

[M01] 读取命令行参数
来源：http://hro.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://rmm.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://iqn.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://pdz.gzhubu.top

TS:   process.argv.slice(2)
来源：http://hem.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://crd.guannengcc.top

Go:   os.Args[1:]
来源：http://kkn.smart0.xyz

Ruby: ARGV
来源：http://obf.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://dsf.snrcjt.cn

[M02] 读取环境变量
来源：http://wum.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://cwq.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dcr.shzxlz.cn

JS:   process.env.HOME
来源：http://mwc.nanxinkj.top

TS:   process.env.HOME
来源：http://omy.jianghu66.top

Java: System.getenv("HOME")
来源：http://qzz.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aou.yuxming.cn

Ruby: ENV["HOME"]
来源：http://krz.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zre.zycfv.cn

[M03] 执行外部命令
来源：http://uhq.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cqt.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://huf.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hmg.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://hai.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://apa.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dly.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zqp.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://sle.andypj.xyz

[M04] 获取当前工作目录
来源：http://hih.mhx1999.top

Py:   os.getcwd()
来源：http://ocw.yueranfly.top

PHP:  getcwd();
来源：http://fhy.yueranfly.top

JS:   process.cwd()
来源：http://uqg.hysaishi.cn

TS:   process.cwd()
来源：http://dph.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://cqz.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://nkw.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://csz.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://auz.hysaishi.cn

[M05] 设置退出码
来源：http://ogn.sysykeji.top

Py:   sys.exit(1)
来源：http://zyl.nwbrower.top

PHP:  exit(1);
来源：http://tzm.epnwcf.com

JS:   process.exit(1)
来源：http://feb.yj20258.top

TS:   process.exit(1)
来源：http://okc.gzhubu.top

Java: System.exit(1)
来源：http://wil.yvedp.cn

Go:   os.Exit(1)
来源：http://yck.wangshuangyany.cn

Ruby: exit 1
来源：http://hfg.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zxh.shanyushiyangtech.top

[M06] 向标准错误输出
来源：http://azw.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://eyu.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://owj.ehwqpu.com

JS:   console.error("err")
来源：http://tln.shangyingyoupin.top

TS:   console.error("err")
来源：http://rsx.hysaishi.cn

Java: System.err.println("err")
来源：http://lho.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jvd.vehdjk.com

Ruby: warn "err"
来源：http://sgz.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://jpb.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://uwr.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://qvd.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cca.xinyue.icu

JS:   require.main === module
来源：http://uah.guannengcc.top

TS:   require.main === module
来源：http://fdh.yj202588.top

Java: public static void main(String[] args)
来源：http://rcb.chenzaomai.com

Go:   func main()
来源：http://ret.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xma.c1oappe.top

C#:   static void Main(string[] args)
来源：http://bqn.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://ttg.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://jzo.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://iab.yonumen.top

JS:   process.platform;  process.version
来源：http://llq.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://iyc.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ghd.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ndh.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zcd.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ori.xuanzx.com

================================================================================
来源：http://yro.ydjk.org.cn

N. 数据结构与算法
来源：http://qlp.jlsjyb.cn

================================================================================
来源：http://hau.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://rpg.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://aaq.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ike.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mzp.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gmb.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gmb.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://mly.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ekl.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://ukw.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://hvc.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://qeu.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://brw.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://mry.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wod.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tjy.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://gjx.fengsongda.top

Ruby: arr.sort
来源：http://jdu.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://lea.yonumen.top

[N03] 快速排序（分治示例）
来源：http://pwx.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ihd.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://gzs.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://txm.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ste.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uxg.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dag.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nyl.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ouc.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://qtz.guowangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jsv.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ezf.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nmm.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iql.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://liu.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://twv.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://guy.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dme.daria6918.cn

[N05] 最大公约数
来源：http://ozb.gzhubu.top

Py:   math.gcd(a, b)
来源：http://vsn.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cyh.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dxa.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kpz.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hnt.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fgr.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://brn.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://apu.fzhhl.top

[N06] 判断回文字符串
来源：http://avv.xuanzx.com

Py:   s == s[::-1]
来源：http://dcw.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://flm.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://mft.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://gpz.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oqn.ybcxt.top

Go:   // 双指针从两端比较
来源：http://gjd.hfpthk.cn

Ruby: s == s.reverse
来源：http://rxj.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hrg.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://pmy.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://foe.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hre.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zhg.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://oie.shzxlz.cn

Java: // 手写 HashMap
来源：http://eia.yonumen.top

Go:   // 手写 map[int]int
来源：http://jhr.cheryme.top

Ruby: // 手写 Hash
来源：http://ouy.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tfc.jinqigfzy.top

[N08] 生成全排列
来源：http://gsc.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://gwu.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://fse.c1oappe.top

JS:   // 手写回溯递归
来源：http://hkg.iojbl.cn

TS:   // 手写回溯递归
来源：http://ylj.cdnleiting.top

Java: // 手写回溯递归
来源：http://inr.yuxming.cn

Go:   // 手写回溯递归
来源：http://krw.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://zeu.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://bkp.hnqzz.top


<!-- 参考信息 -->