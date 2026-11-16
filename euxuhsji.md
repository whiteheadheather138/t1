代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dgz.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sgg.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fvp.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xhb.meibo888.top

================================================================================
来源：http://ilg.uphjek.com

K. JSON 与序列化
来源：http://rxv.c1oappe.top

================================================================================
来源：http://voo.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://stv.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nvh.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://juc.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://vdf.uphjek.com

TS:   JSON.stringify(obj)
来源：http://ozz.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ass.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://ois.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jdp.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bzn.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://tza.yueranfly.top

Py:   json.loads(s)
来源：http://fzb.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rbo.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://rnd.yj20258888.top

TS:   JSON.parse(s)
来源：http://ubt.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://utl.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://vwl.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://oqu.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yeu.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://beb.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lez.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mle.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zee.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://lql.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wnt.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jri.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gwn.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://awc.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://tlz.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wvv.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jmd.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgo.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bwi.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://orm.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hpc.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wez.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://flu.hnxiangtu.top

[K05] 深拷贝对象
来源：http://eqo.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://mqc.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://gcj.daria6918.cn

JS:   structuredClone(obj)
来源：http://wil.yonumen.top

TS:   structuredClone(obj)
来源：http://onx.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://dhs.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sxg.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lsy.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tmk.ydzc1.top

[K06] 解析 URL 查询串
来源：http://msi.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wcd.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gnw.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cfu.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mwi.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xjb.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hrr.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://unv.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jbk.zdqjudy.top

[K07] 进制转换
来源：http://njn.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://utx.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ljf.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://izl.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://guq.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vku.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ida.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://two.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://npx.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qds.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://gsa.zhijiandao.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lvv.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://txw.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://mdq.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nsk.cheryme.top

Go:   encoding/gob
来源：http://zxt.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://acm.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bfc.hysaishi.cn

================================================================================
来源：http://dxd.jianghu66.top

L. 网络请求
来源：http://gts.ehwqpu.com

================================================================================
来源：http://fzx.yj20258.top

[L01] 发送 GET 请求
来源：http://wjh.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sfn.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pkk.dashuyun.cn

JS:   await fetch(url)
来源：http://ouh.hammf.cn

TS:   await fetch(url)
来源：http://efs.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oyo.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://fkw.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ntf.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wse.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://mjv.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://scx.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ars.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfv.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rdq.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gfm.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://udq.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nek.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lqy.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://imh.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lfo.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jjr.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ygw.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydk.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kxk.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pfo.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://thf.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://smp.yj202588.top

[L04] 设置超时
来源：http://kkr.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://fco.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://stn.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://atg.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kte.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lvp.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lha.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iyh.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wix.yj20258.top

[L05] 上传文件（multipart）
来源：http://xju.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dyg.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tjv.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ick.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uep.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jiw.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ohn.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://czc.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vqs.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://iwd.daxiang520.top

Py:   resp.json()
来源：http://xpl.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://etb.shanyushiyangtech.top

JS:   await resp.json()
来源：http://jtc.daxiang520.top

TS:   await resp.json()
来源：http://dmi.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rvm.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uph.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://xoe.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ktr.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://urz.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qri.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qgg.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://xfi.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://ybp.sweek.top

Java: resp.statusCode()
来源：http://tpp.zdqjudy.top

Go:   resp.StatusCode
来源：http://qkp.tian-w.cn

Ruby: resp.code.to_i
来源：http://elz.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://koa.daxiang520.top

[L08] 并发请求多个地址
来源：http://fir.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zxq.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://pxa.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jor.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gkx.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zzr.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zpq.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zwp.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhh.tarul.cn

================================================================================
来源：http://rpu.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://mrc.zhijiandao.cn

================================================================================
来源：http://cwg.chenzaomai.com

[M01] 读取命令行参数
来源：http://fum.sxryk.cn

Py:   sys.argv[1:]
来源：http://rbo.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://mpb.hesvh.cn

JS:   process.argv.slice(2)
来源：http://nnp.jianghu66.top

TS:   process.argv.slice(2)
来源：http://cij.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://ikq.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://suv.zycfv.cn

Ruby: ARGV
来源：http://cnb.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://uuf.yuxming.cn

[M02] 读取环境变量
来源：http://ywe.cashguo.top

Py:   os.environ.get("HOME")
来源：http://iln.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vzm.tanke756.top

JS:   process.env.HOME
来源：http://mqf.yfazqb.com

TS:   process.env.HOME
来源：http://shx.ehwqpu.com

Java: System.getenv("HOME")
来源：http://hdv.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mpr.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://sax.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qid.sjlbkw.cn

[M03] 执行外部命令
来源：http://reh.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://psz.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wce.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jlo.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zmk.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bar.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kjq.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://uui.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://qzj.ydzc1.top

[M04] 获取当前工作目录
来源：http://gzg.tarul.cn

Py:   os.getcwd()
来源：http://hgy.chenzaomai.com

PHP:  getcwd();
来源：http://qox.sufxvd.cn

JS:   process.cwd()
来源：http://lvq.316326.xyz

TS:   process.cwd()
来源：http://frm.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://nom.0kj1m.cn

Go:   os.Getwd()
来源：http://kcc.daxiang520.top

Ruby: Dir.pwd
来源：http://lfo.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://xmg.tianlin.xyz

[M05] 设置退出码
来源：http://flz.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://ano.xylfe.cn

PHP:  exit(1);
来源：http://tur.jyoumei.cn

JS:   process.exit(1)
来源：http://scw.dianchejie.cn

TS:   process.exit(1)
来源：http://pva.yanxiufei.cn

Java: System.exit(1)
来源：http://tox.zdbjq.cn

Go:   os.Exit(1)
来源：http://fqe.nanxinkj.top

Ruby: exit 1
来源：http://hcr.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://drx.wangdashe.top

[M06] 向标准错误输出
来源：http://ymi.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://esv.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://slw.epnwcf.com

JS:   console.error("err")
来源：http://yaz.ehwqpu.com

TS:   console.error("err")
来源：http://glf.fengsongda.top

Java: System.err.println("err")
来源：http://lwt.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rdv.xinyue.icu

Ruby: warn "err"
来源：http://erp.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://xye.yongpay.top

[M07] 判断是否为主入口
来源：http://ykh.jinqigfzy.top

Py:   if __name__ == "__main__":
来源：http://gxd.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://soe.jinqigfzy.top

JS:   require.main === module
来源：http://esz.cucudq.cn

TS:   require.main === module
来源：http://ixh.guowangkeji.top

Java: public static void main(String[] args)
来源：http://vry.chenzaomai.com

Go:   func main()
来源：http://nky.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fqk.tanke756.top

C#:   static void Main(string[] args)
来源：http://lsm.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://qbo.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://gvx.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://ewk.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://nps.dianchejie.cn

TS:   process.platform;  process.version
来源：http://xvd.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mou.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mqo.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://idj.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://ytl.bjfxy.top

================================================================================
来源：http://fnv.cashguo.top

N. 数据结构与算法
来源：http://rck.chenjidiqi.icu

================================================================================
来源：http://tix.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://kzl.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://svq.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ixb.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zup.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hov.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://xev.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://dke.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://whn.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://scb.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://ucm.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://llt.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jzm.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://fkk.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vjq.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nbn.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://wcw.zdqjudy.top

Ruby: arr.sort
来源：http://mgb.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ptu.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://ptf.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wva.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://ywl.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qcn.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gdx.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mgw.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baa.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zxw.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dld.jiagoushi.top

[N04] 斐波那契数列
来源：http://msj.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nia.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mdl.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://imv.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://coq.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trh.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xtc.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dth.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wmh.xziqi.cn

[N05] 最大公约数
来源：http://npp.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://uqo.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ovo.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jzi.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ecw.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ags.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sqs.bbcook.cn

Ruby: a.gcd(b)
来源：http://qrc.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://huv.bbcook.cn

[N06] 判断回文字符串
来源：http://wis.daxiang520.top

Py:   s == s[::-1]
来源：http://uiv.iojbl.cn

PHP:  $s === strrev($s);
来源：http://zor.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://wdx.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://evc.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ulh.ybcxt.top

Go:   // 双指针从两端比较
来源：http://qmh.vehdjk.com

Ruby: s == s.reverse
来源：http://rgy.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pec.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://knf.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hjt.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://spj.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nsl.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://sgt.pycfn.com

Java: // 手写 HashMap
来源：http://cxo.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://zwl.fengsongda.top

Ruby: // 手写 Hash
来源：http://rqu.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rxc.nwbrower.top

[N08] 生成全排列
来源：http://wpq.birdmap.top

Py:   itertools.permutations(arr)
来源：http://flo.yongpay.top

PHP:  // 手写递归交换
来源：http://nzb.sxryk.cn

JS:   // 手写回溯递归
来源：http://bbc.zhengqikj.top

TS:   // 手写回溯递归
来源：http://tgq.ctjpmb.com


<!-- 参考信息 -->