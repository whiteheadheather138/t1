代发 wailian999

================================================================================
来源：http://ctp.hesvh.cn

K. JSON 与序列化
来源：http://wth.fzhhl.top

================================================================================
来源：http://kkd.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://xyw.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yog.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ugd.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://iej.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://alw.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dep.tanke756.top

Go:   json.Marshal(obj)
来源：http://xos.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mxh.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hug.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://xta.sufxvd.cn

Py:   json.loads(s)
来源：http://odp.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tvx.yueranfly.top

JS:   JSON.parse(s)
来源：http://mbm.uphjek.com

TS:   JSON.parse(s)
来源：http://akn.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ubv.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://sxm.daxiang520.top

Ruby: JSON.parse(s)
来源：http://elj.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zqx.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://eso.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uhc.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://txi.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mdi.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yll.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kjf.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pls.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://rot.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wqi.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://vqu.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://utb.yj202588.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dig.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hap.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ncr.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mdv.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yim.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vfj.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wed.tarul.cn

[K05] 深拷贝对象
来源：http://rpw.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://jmf.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://lzx.yangfankeji.com

JS:   structuredClone(obj)
来源：http://fuv.chenzaomai.com

TS:   structuredClone(obj)
来源：http://nlj.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lpt.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tlu.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uzf.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hhe.guannengcc.top

[K06] 解析 URL 查询串
来源：http://jnp.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ghn.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://apn.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qrq.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ank.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://owi.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rej.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tdw.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gmf.yj20258.top

[K07] 进制转换
来源：http://mov.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rpq.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eac.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ivd.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ipc.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://crm.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cub.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tqe.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jlo.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://auv.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://ofg.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nwh.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://lha.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://jgj.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ocr.jinghuilouyu.cn

Go:   encoding/gob
来源：http://xdx.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://ypn.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lqk.mhx1999.top

================================================================================
来源：http://spo.gotoacloud.top

L. 网络请求
来源：http://pfq.daria6918.cn

================================================================================
来源：http://hrn.hammf.cn

[L01] 发送 GET 请求
来源：http://spz.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vkx.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rhr.haohaochexian.top

JS:   await fetch(url)
来源：http://uvf.vehdjk.com

TS:   await fetch(url)
来源：http://jvk.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vat.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://hml.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://glo.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ayz.dashuyun.cn

[L02] 发送 POST JSON
来源：http://vpe.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://xxr.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xei.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://swk.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gcn.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://czm.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://art.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tlt.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tei.yongpay.top

[L03] 设置自定义请求头
来源：http://evt.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cgw.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cby.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://obg.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rvy.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://run.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uds.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zic.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mav.quarkkingdee.top

[L04] 设置超时
来源：http://wmo.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://xzj.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://usl.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cbx.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwf.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://plt.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xuq.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xad.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xmg.nwbrower.top

[L05] 上传文件（multipart）
来源：http://mme.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sfr.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ssg.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rmj.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oaf.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://srz.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vpr.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ubj.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bmv.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://iwa.ctjpmb.com

Py:   resp.json()
来源：http://zru.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://inu.c1oappe.top

JS:   await resp.json()
来源：http://orn.uphjek.com

TS:   await resp.json()
来源：http://znm.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lwp.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bfh.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://qcp.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dib.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://hap.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jbx.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hqy.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://vfq.cashguo.top

TS:   resp.ok;  resp.status
来源：http://hhk.jqgfzy.top

Java: resp.statusCode()
来源：http://fkt.ivvv.top

Go:   resp.StatusCode
来源：http://vhm.snrcjt.cn

Ruby: resp.code.to_i
来源：http://etf.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://wqr.316326.xyz

[L08] 并发请求多个地址
来源：http://fxj.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dhf.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://ivb.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lvg.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjf.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://apu.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ccx.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ezx.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vly.kuanghao11.cn

================================================================================
来源：http://iul.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://scb.nanxuanxn.top

================================================================================
来源：http://jdy.aizwys.cn

[M01] 读取命令行参数
来源：http://tfn.c1oappe.top

Py:   sys.argv[1:]
来源：http://pdg.fehbvm.com

PHP:  $argv;  $argc;
来源：http://gqb.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://tbo.meibo888.top

TS:   process.argv.slice(2)
来源：http://fvj.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://fqq.tianlin.xyz

Go:   os.Args[1:]
来源：http://eqe.sweek.top

Ruby: ARGV
来源：http://twm.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://oaz.daria6918.cn

[M02] 读取环境变量
来源：http://exz.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://qvi.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xfy.nwbrower.top

JS:   process.env.HOME
来源：http://beo.chenlongwang.top

TS:   process.env.HOME
来源：http://ifr.tian-w.cn

Java: System.getenv("HOME")
来源：http://nlv.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aam.cucudq.cn

Ruby: ENV["HOME"]
来源：http://gec.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jip.xinyue.icu

[M03] 执行外部命令
来源：http://zyj.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hvj.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uon.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qyd.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xkx.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cuj.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pch.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://rxm.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://oni.fengsongda.top

[M04] 获取当前工作目录
来源：http://wos.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://rln.zycfv.cn

PHP:  getcwd();
来源：http://ejv.nwbrower.top

JS:   process.cwd()
来源：http://gez.svipenyu.cn

TS:   process.cwd()
来源：http://oqv.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://txq.birdmap.top

Go:   os.Getwd()
来源：http://hph.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://yiu.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://pnq.ppjwa.cn

[M05] 设置退出码
来源：http://hag.cheryme.top

Py:   sys.exit(1)
来源：http://ziu.pengpengdd.cyou

PHP:  exit(1);
来源：http://ozj.pengpengdd.cyou

JS:   process.exit(1)
来源：http://oyf.havefunace.top

TS:   process.exit(1)
来源：http://aai.yangfankeji.com

Java: System.exit(1)
来源：http://mem.zhixingplan.top

Go:   os.Exit(1)
来源：http://vqg.sxryk.cn

Ruby: exit 1
来源：http://oqw.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wrf.ybcxt.top

[M06] 向标准错误输出
来源：http://cdx.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://tig.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sfc.ppjwa.cn

JS:   console.error("err")
来源：http://gxr.hfpthk.cn

TS:   console.error("err")
来源：http://aeu.aibaodan.cn

Java: System.err.println("err")
来源：http://syx.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uen.hesvh.cn

Ruby: warn "err"
来源：http://dtq.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://iqe.yuxming.cn

[M07] 判断是否为主入口
来源：http://avh.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://qkn.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kdi.haohaochexian.top

JS:   require.main === module
来源：http://vgi.0kj1m.cn

TS:   require.main === module
来源：http://ugr.andypj.xyz

Java: public static void main(String[] args)
来源：http://zpv.epnwcf.com

Go:   func main()
来源：http://llt.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://azg.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://fpj.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://grj.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://pez.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://eyo.iojbl.cn

JS:   process.platform;  process.version
来源：http://cjl.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://rwm.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aqp.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ktu.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fmw.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://atx.zhongyouzk.top

================================================================================
来源：http://syt.kuanghao11.cn

N. 数据结构与算法
来源：http://ymq.zdbjq.cn

================================================================================
来源：http://lei.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://ayt.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://dti.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wsl.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oez.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uab.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://lik.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://vth.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vkh.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://wvg.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://eag.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://lko.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://unm.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yny.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vyy.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qin.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://duu.yvedp.cn

Ruby: arr.sort
来源：http://tvf.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tak.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://dhx.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nqx.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://msd.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hby.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://thj.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ybw.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dfb.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xer.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pto.yangfankeji.com

[N04] 斐波那契数列
来源：http://quv.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wmb.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://omb.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rdl.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jcg.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://juq.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rlf.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bnw.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bji.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://cni.tarul.cn

Py:   math.gcd(a, b)
来源：http://xmt.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vea.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvo.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aju.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://llz.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vmy.ybcxt.top

Ruby: a.gcd(b)
来源：http://gww.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xhn.pycfn.com

[N06] 判断回文字符串
来源：http://pjf.jqgufenzy.top

Py:   s == s[::-1]
来源：http://xzl.yonumen.top

PHP:  $s === strrev($s);
来源：http://irt.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://xyw.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://vmr.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hwd.pycfn.com

Go:   // 双指针从两端比较
来源：http://tvr.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://qme.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fuq.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://ivk.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://orf.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iyn.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vyo.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://zir.zycfv.cn

Java: // 手写 HashMap
来源：http://lio.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://jot.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://xis.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ixu.zdqjudy.top

[N08] 生成全排列
来源：http://hvz.cashguo.top

Py:   itertools.permutations(arr)
来源：http://qmw.epnwcf.com

PHP:  // 手写递归交换
来源：http://pus.ivvv.top

JS:   // 手写回溯递归
来源：http://reg.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://pod.gogol.net.cn

Java: // 手写回溯递归
来源：http://lwi.yj20258888.top

Go:   // 手写回溯递归
来源：http://nqv.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://uuz.yj202588.top

C#:   // 手写回溯递归
来源：http://jah.shangyingyoupin.top


<!-- 参考信息 -->