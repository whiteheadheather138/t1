代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://acx.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nbw.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://one.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hvs.haohaochexian.top

================================================================================
来源：http://bif.ivvv.top

K. JSON 与序列化
来源：http://ygt.birdmap.top

================================================================================
来源：http://azc.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://flv.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pcm.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bzs.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://scb.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://uym.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://riw.yonumen.top

Go:   json.Marshal(obj)
来源：http://rgv.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xiz.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nql.havefunace.top

[K02] JSON 字符串转对象
来源：http://ksj.tarul.cn

Py:   json.loads(s)
来源：http://swd.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qsp.316326.xyz

JS:   JSON.parse(s)
来源：http://cbq.52xcode.cn

TS:   JSON.parse(s)
来源：http://ami.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pfc.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://znt.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://xnd.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://osz.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://jcw.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rwl.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hjx.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://hay.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hom.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wvl.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zil.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://kdh.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kbc.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://wfu.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vcr.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://obc.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mmz.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nmz.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://agz.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uvk.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vdq.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://srl.quarkkingdee.top

[K05] 深拷贝对象
来源：http://rdi.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://ydw.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://soa.birdmap.top

JS:   structuredClone(obj)
来源：http://mtt.shuidangran.top

TS:   structuredClone(obj)
来源：http://xzr.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://scy.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mgb.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://heo.cheryme.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oon.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://ugf.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xdg.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ord.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pje.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rwp.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qbt.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://brp.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dhg.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://unx.birdmap.top

[K07] 进制转换
来源：http://btb.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kee.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uno.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://egi.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fua.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wnm.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qwg.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pre.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tje.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://pmq.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://mwa.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://fxp.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://xpp.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://tgy.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://adi.hongshengwenyu.top

Go:   encoding/gob
来源：http://ycx.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://fex.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ilh.havefunace.top

================================================================================
来源：http://xnu.havefunace.top

L. 网络请求
来源：http://ozj.dianchejie.cn

================================================================================
来源：http://lsg.vehdjk.com

[L01] 发送 GET 请求
来源：http://qzx.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://toe.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://koa.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://ufn.ydjk.org.cn

TS:   await fetch(url)
来源：http://gsv.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cov.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://dda.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://swr.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hpt.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://dan.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://kma.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sdt.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dvp.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gsl.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gez.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jdq.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ocl.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kpc.yueranfly.top

[L03] 设置自定义请求头
来源：http://gsx.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rbk.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ocy.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tea.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cjq.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://phx.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://irk.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ray.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://szo.yfazqb.com

[L04] 设置超时
来源：http://pdu.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://jom.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wlr.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdl.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ihz.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bkf.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://imc.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rut.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qbc.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://dyq.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nmd.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://klh.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://onp.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mcu.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qak.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vny.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ujw.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xup.sweek.top

[L06] 解析响应为 JSON
来源：http://tui.chenzaomai.com

Py:   resp.json()
来源：http://vjc.pycfn.com

PHP:  json_decode($body, true);
来源：http://lqo.jianghu66.top

JS:   await resp.json()
来源：http://lcs.shangyingyoupin.top

TS:   await resp.json()
来源：http://hgh.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xwv.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tul.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://oys.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vjb.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://ers.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lot.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yfh.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://yjv.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://snd.ppjwa.cn

Java: resp.statusCode()
来源：http://rcw.chenlongwang.top

Go:   resp.StatusCode
来源：http://cgc.xylfe.cn

Ruby: resp.code.to_i
来源：http://apm.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://ety.nanxinkj.top

[L08] 并发请求多个地址
来源：http://ygu.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://msb.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://brl.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lza.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fjg.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hiu.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iwk.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ncd.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aah.fanxiaobao.xyz

================================================================================
来源：http://tba.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://omf.uphjek.com

================================================================================
来源：http://sge.xziqi.cn

[M01] 读取命令行参数
来源：http://xtv.zycfv.cn

Py:   sys.argv[1:]
来源：http://muh.fengsongda.top

PHP:  $argv;  $argc;
来源：http://veb.meibo888.top

JS:   process.argv.slice(2)
来源：http://hnq.fengsongda.top

TS:   process.argv.slice(2)
来源：http://kti.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://qdv.jinqigfzy.top

Go:   os.Args[1:]
来源：http://vcf.xinyue.icu

Ruby: ARGV
来源：http://sac.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://hov.birdmap.top

[M02] 读取环境变量
来源：http://kfw.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://bne.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uku.hysaishi.cn

JS:   process.env.HOME
来源：http://gyd.jianghu66.top

TS:   process.env.HOME
来源：http://mfq.bjfxy.top

Java: System.getenv("HOME")
来源：http://uqm.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sgi.yj20258888.top

Ruby: ENV["HOME"]
来源：http://bem.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ugj.aibaodan.cn

[M03] 执行外部命令
来源：http://upf.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zdb.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dav.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rnv.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://zun.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mfi.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://llb.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://arj.epnwcf.com

C#:   Process.Start("ls", "-l");
来源：http://mxp.jinqigufen.top

[M04] 获取当前工作目录
来源：http://bpy.chenjidiqi.icu

Py:   os.getcwd()
来源：http://bjz.pycfn.com

PHP:  getcwd();
来源：http://egy.hammf.cn

JS:   process.cwd()
来源：http://dpn.xylfe.cn

TS:   process.cwd()
来源：http://sqg.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://cum.sufxvd.cn

Go:   os.Getwd()
来源：http://pkf.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://kgk.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://bnq.tian-w.cn

[M05] 设置退出码
来源：http://aym.tarul.cn

Py:   sys.exit(1)
来源：http://sss.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://wws.quarkkingdee.top

JS:   process.exit(1)
来源：http://ial.birdmap.top

TS:   process.exit(1)
来源：http://wtn.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://fsb.0kj1m.cn

Go:   os.Exit(1)
来源：http://jxs.nanxinkj.top

Ruby: exit 1
来源：http://gma.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rgw.yj20258.top

[M06] 向标准错误输出
来源：http://rix.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://zxq.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://djh.tarul.cn

JS:   console.error("err")
来源：http://jro.jinqigufen.top

TS:   console.error("err")
来源：http://uiq.c1oappe.top

Java: System.err.println("err")
来源：http://woa.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ufp.vqdsnc.cn

Ruby: warn "err"
来源：http://lod.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://nep.fanxiaobao.xyz

[M07] 判断是否为主入口
来源：http://qhv.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://pcf.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fhy.sufxvd.cn

JS:   require.main === module
来源：http://may.jyoumei.cn

TS:   require.main === module
来源：http://hpy.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://zqn.birdmap.top

Go:   func main()
来源：http://jjs.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nry.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://xyl.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://gav.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://lsc.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://eql.aibaodan.cn

JS:   process.platform;  process.version
来源：http://nqh.c1oappe.top

TS:   process.platform;  process.version
来源：http://bkx.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ahm.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://end.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xyl.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://jhn.hcnkem.com

================================================================================
来源：http://uqt.tanke756.top

N. 数据结构与算法
来源：http://zga.pengpengdd.cyou

================================================================================
来源：http://hcg.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://oua.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://hnv.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hgy.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://isg.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zyf.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://xgn.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://hjg.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://gmv.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://kow.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://tfx.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://sef.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iiw.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://atn.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://uah.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bye.hammf.cn

Go:   slices.Sort(arr)
来源：http://wvr.hnxiangtu.top

Ruby: arr.sort
来源：http://xhi.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sur.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://azu.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kob.xinyue.icu

PHP:  // 递归实现，或用 usort
来源：http://six.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nvy.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xdb.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://njt.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sts.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jla.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://pyb.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://glg.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://npp.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mrt.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yca.ctjpmb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pwp.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://igq.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oxe.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qzy.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ldq.guannengcc.top

[N05] 最大公约数
来源：http://jrf.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://tnq.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://htp.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ncv.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qyr.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://agp.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cka.guowangkeji.top

Ruby: a.gcd(b)
来源：http://mba.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qau.ybcxt.top

[N06] 判断回文字符串
来源：http://mgi.yonumen.top

Py:   s == s[::-1]
来源：http://xux.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://hpq.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://yxw.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://cvj.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://klg.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://udp.yj20258888.top

Ruby: s == s.reverse
来源：http://kny.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lsh.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://gzg.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ecn.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ond.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xvw.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://ecy.bbcook.cn

Java: // 手写 HashMap
来源：http://uyc.fengsongda.top

Go:   // 手写 map[int]int
来源：http://ccg.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://uob.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://wnq.pycfn.com

[N08] 生成全排列
来源：http://djl.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://vcp.cucudq.cn

PHP:  // 手写递归交换
来源：http://hbt.epnwcf.com

JS:   // 手写回溯递归
来源：http://anj.guannengcc.top

TS:   // 手写回溯递归
来源：http://fcr.yanxiufei.cn


<!-- 参考信息 -->