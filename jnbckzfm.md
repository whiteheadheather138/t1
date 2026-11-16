代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ovp.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hgn.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nrg.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://ezf.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ubu.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pnc.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rlm.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sci.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ial.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xyx.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dzu.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rel.havefunace.top

================================================================================
来源：http://aqh.tianlin.xyz

K. JSON 与序列化
来源：http://lmm.hywenlv.cn

================================================================================
来源：http://ybo.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://qmk.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ibq.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wki.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://rpy.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://weu.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qfe.tian-w.cn

Go:   json.Marshal(obj)
来源：http://ick.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://wfi.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dzn.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://axk.svipenyu.cn

Py:   json.loads(s)
来源：http://mqe.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dru.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://xco.chenzaomai.com

TS:   JSON.parse(s)
来源：http://wuu.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uek.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://kkv.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://lwp.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://awk.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://kux.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ccd.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dtr.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tvv.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fxl.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ydo.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hwu.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://xmp.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bvh.jinyuanbaomall.cn

[K04] 读取 JSON 文件
来源：http://ziy.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pqk.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dlh.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bde.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xub.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://irb.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zmv.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cbg.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zmq.nanxuanxn.top

[K05] 深拷贝对象
来源：http://zir.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://bsv.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://uif.yj202588.top

JS:   structuredClone(obj)
来源：http://zqz.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://bmi.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vxk.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hjt.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hyd.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ugq.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://uus.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://him.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ntg.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pgq.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://khp.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ekr.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dsg.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wsd.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxz.zdqjudy.top

[K07] 进制转换
来源：http://noa.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ref.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mhs.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://chp.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://stq.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ifd.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wza.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mxk.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://igt.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://svk.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://btx.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nde.hnxiangtu.top

JS:   v8.serialize(obj)        // Node
来源：http://qeq.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://fif.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ywa.sxryk.cn

Go:   encoding/gob
来源：http://uyq.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://ncy.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jsr.zhongyouzk.top

================================================================================
来源：http://zri.dashuyun.cn

L. 网络请求
来源：http://ddo.nanxinkj.top

================================================================================
来源：http://uke.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://ihc.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xgk.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hfa.yj20258888.top

JS:   await fetch(url)
来源：http://sjf.snrcjt.cn

TS:   await fetch(url)
来源：http://pfa.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rfe.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://ext.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lev.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dam.cqqwz.cn

[L02] 发送 POST JSON
来源：http://dbk.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://chk.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cql.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zro.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hfv.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hfc.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fki.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://trx.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mde.andypj.xyz

[L03] 设置自定义请求头
来源：http://lao.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rns.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ncq.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ued.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bug.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nyx.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jhz.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sus.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://puo.shzxlz.cn

[L04] 设置超时
来源：http://xsi.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://bxl.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bgc.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zvu.jyoumei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdm.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qun.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kfh.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zim.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ekt.ydzc1.top

[L05] 上传文件（multipart）
来源：http://lmv.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kso.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lxl.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qvl.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lsg.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bec.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uat.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uat.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mic.sxryk.cn

[L06] 解析响应为 JSON
来源：http://oep.316326.xyz

Py:   resp.json()
来源：http://vlu.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://ccd.yonumen.top

JS:   await resp.json()
来源：http://cyc.0kj1m.cn

TS:   await resp.json()
来源：http://vcb.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mdu.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zzi.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://gnr.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dbx.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://fhy.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://clu.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gin.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://ike.meibo888.top

TS:   resp.ok;  resp.status
来源：http://xqo.ydjk.org.cn

Java: resp.statusCode()
来源：http://fez.hcnkem.com

Go:   resp.StatusCode
来源：http://nrz.xinyue.icu

Ruby: resp.code.to_i
来源：http://gei.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://xim.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://tsv.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nbx.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://qbr.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxb.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hku.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eli.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bqv.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ecr.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fxj.hnxiangtu.top

================================================================================
来源：http://qgx.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://trd.shangyingyoupin.top

================================================================================
来源：http://amv.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://tpo.hfpthk.cn

Py:   sys.argv[1:]
来源：http://clb.redwolf501.top

PHP:  $argv;  $argc;
来源：http://fkz.hnqzz.top

JS:   process.argv.slice(2)
来源：http://uca.cucudq.cn

TS:   process.argv.slice(2)
来源：http://fdd.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://gwy.daxiang520.top

Go:   os.Args[1:]
来源：http://awi.havefunace.top

Ruby: ARGV
来源：http://srw.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://lzw.cucudq.cn

[M02] 读取环境变量
来源：http://fcy.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://sxt.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qft.sysykeji.top

JS:   process.env.HOME
来源：http://qnx.shangyingyoupin.top

TS:   process.env.HOME
来源：http://axt.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://rqy.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qgt.andypj.xyz

Ruby: ENV["HOME"]
来源：http://poc.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cor.iojbl.cn

[M03] 执行外部命令
来源：http://vir.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hre.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://icf.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kmn.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qwx.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dfu.shuidangran.top

Go:   exec.Command("ls", "-l").Output()
来源：http://aev.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://htw.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://dbo.fktsv.cn

[M04] 获取当前工作目录
来源：http://kdz.9152youxi.cn

Py:   os.getcwd()
来源：http://wzy.gzhubu.top

PHP:  getcwd();
来源：http://azy.jinqigfzy.top

JS:   process.cwd()
来源：http://ntp.hywenlv.cn

TS:   process.cwd()
来源：http://rky.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://xuw.yanxiufei.cn

Go:   os.Getwd()
来源：http://zje.aizwys.cn

Ruby: Dir.pwd
来源：http://rto.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kgr.jqgfzy.top

[M05] 设置退出码
来源：http://bub.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://ytt.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://fcw.andypj.xyz

JS:   process.exit(1)
来源：http://aba.yanxiufei.cn

TS:   process.exit(1)
来源：http://czs.wangdashe.top

Java: System.exit(1)
来源：http://ozg.zhijiandao.cn

Go:   os.Exit(1)
来源：http://rci.shanyushiyangtech.top

Ruby: exit 1
来源：http://gxi.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hdf.gotoacloud.top

[M06] 向标准错误输出
来源：http://utl.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://kdb.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://osa.epnwcf.com

JS:   console.error("err")
来源：http://aab.yvedp.cn

TS:   console.error("err")
来源：http://ywq.hammf.cn

Java: System.err.println("err")
来源：http://fit.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wjn.cashguo.top

Ruby: warn "err"
来源：http://dnx.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://sgs.gogol.net.cn

[M07] 判断是否为主入口
来源：http://gfj.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://tgg.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kdq.smart0.xyz

JS:   require.main === module
来源：http://ntm.xziqi.cn

TS:   require.main === module
来源：http://phv.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://ofc.hysaishi.cn

Go:   func main()
来源：http://eks.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://knm.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://jxq.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://zjv.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://vya.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://edq.9152youxi.cn

JS:   process.platform;  process.version
来源：http://zub.hammf.cn

TS:   process.platform;  process.version
来源：http://uzf.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fru.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://itn.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jtd.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nra.fengsongda.top

================================================================================
来源：http://rkc.cqqwz.cn

N. 数据结构与算法
来源：http://nrq.fktsv.cn

================================================================================
来源：http://svd.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://gao.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://pqx.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ttu.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kwd.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tsl.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://qup.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://ajv.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ebt.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tqw.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://oor.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://fkh.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tcw.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jpt.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ecv.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rcz.hnqzz.top

Go:   slices.Sort(arr)
来源：http://zbq.yj202588.top

Ruby: arr.sort
来源：http://ipy.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hug.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://uby.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lfs.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://wkc.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://icf.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xdv.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qek.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dik.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cxy.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://xin.smart0.xyz

[N04] 斐波那契数列
来源：http://yci.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dqp.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qln.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://muo.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mxz.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bpe.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nfd.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://btd.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tnd.xuanzx.com

[N05] 最大公约数
来源：http://ohw.shuidangran.top

Py:   math.gcd(a, b)
来源：http://ykh.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sko.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yni.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://our.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hoz.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xfg.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://own.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lek.ctjpmb.com

[N06] 判断回文字符串
来源：http://nin.haohaochexian.top

Py:   s == s[::-1]
来源：http://jnw.sysykeji.top

PHP:  $s === strrev($s);
来源：http://wli.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://xia.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://cys.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lbd.daxiang520.top

Go:   // 双指针从两端比较
来源：http://qck.yvedp.cn

Ruby: s == s.reverse
来源：http://tuz.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zih.hammf.cn

[N07] 两数之和（返回下标）
来源：http://hht.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://krx.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zbu.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bca.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://wif.svipenyu.cn

Java: // 手写 HashMap
来源：http://crg.haohaochexian.top


<!-- 参考信息 -->