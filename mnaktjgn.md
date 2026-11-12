代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qwf.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yvp.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jsw.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nxk.hfpthk.cn

================================================================================
来源：http://nni.cashguo.top

K. JSON 与序列化
来源：http://hnq.yfazqb.com

================================================================================
来源：http://xht.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://nfg.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jvv.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hpa.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://fkh.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://qkv.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gxc.xinyue.icu

Go:   json.Marshal(obj)
来源：http://yzp.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://xkj.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tfs.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://dqj.jinqigufen.top

Py:   json.loads(s)
来源：http://gvy.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ujn.snrcjt.cn

JS:   JSON.parse(s)
来源：http://lsn.jyoumei.cn

TS:   JSON.parse(s)
来源：http://clu.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xrj.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://gqk.cucudq.cn

Ruby: JSON.parse(s)
来源：http://bgm.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hgj.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://iha.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wzq.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vof.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kdc.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bab.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wuk.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hwp.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hds.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zyb.uphjek.com

[K04] 读取 JSON 文件
来源：http://xof.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rfg.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://for.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eyi.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rhf.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rvc.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cay.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xms.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pvq.ybcxt.top

[K05] 深拷贝对象
来源：http://jdt.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://uwf.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://jwo.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://anr.svipenyu.cn

TS:   structuredClone(obj)
来源：http://vqu.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xyt.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cgb.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zjg.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ddm.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://gwm.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mfc.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hry.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fid.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fcu.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://chy.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zrz.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ntw.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uzx.zdqjudy.top

[K07] 进制转换
来源：http://xzg.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eir.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ojz.daria6918.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gix.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yel.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xae.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hpm.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tvr.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vye.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://yxn.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://gmf.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gak.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://fis.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://pal.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ijc.zhiwuduotai.top

Go:   encoding/gob
来源：http://ivp.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://scu.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tts.meibo888.top

================================================================================
来源：http://zqt.yfazqb.com

L. 网络请求
来源：http://kng.hcnkem.com

================================================================================
来源：http://gxm.hnqzz.top

[L01] 发送 GET 请求
来源：http://tfi.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://drr.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://krw.guannengcc.top

JS:   await fetch(url)
来源：http://qye.yuxming.cn

TS:   await fetch(url)
来源：http://hia.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://duv.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://kkm.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://hom.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bot.ehwqpu.com

[L02] 发送 POST JSON
来源：http://fch.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://bmv.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eie.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yfl.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aef.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xus.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ccy.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://osc.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xot.yuxming.cn

[L03] 设置自定义请求头
来源：http://pmf.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vft.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fuz.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxx.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nvm.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://phs.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tpg.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://les.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vtw.yonumen.top

[L04] 设置超时
来源：http://epc.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://opn.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://muv.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkd.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://btr.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uup.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cpm.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cwd.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hcv.cucudq.cn

[L05] 上传文件（multipart）
来源：http://toi.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://auh.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ebj.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fvj.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oqw.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qot.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jhd.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ial.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hax.wangdashe.top

[L06] 解析响应为 JSON
来源：http://lhb.yangfankeji.com

Py:   resp.json()
来源：http://wlv.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://moj.yangfankeji.com

JS:   await resp.json()
来源：http://cbn.shanyushiyangtech.top

TS:   await resp.json()
来源：http://ynl.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rvm.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ezx.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://odg.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://und.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://ypy.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bcy.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fqn.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://crg.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://opi.xuanzx.com

Java: resp.statusCode()
来源：http://wuo.zdqjudy.top

Go:   resp.StatusCode
来源：http://fue.svipenyu.cn

Ruby: resp.code.to_i
来源：http://jzv.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://qte.smart0.xyz

[L08] 并发请求多个地址
来源：http://zrc.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mif.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://uhd.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ijl.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sik.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ybe.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kwu.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qyp.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://chy.zhengqikj.top

================================================================================
来源：http://vzi.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://kwn.hongshengwenyu.top

================================================================================
来源：http://sfe.hcnkem.com

[M01] 读取命令行参数
来源：http://jhn.guowangkeji.top

Py:   sys.argv[1:]
来源：http://vll.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://gef.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://uvb.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://rfh.cheryme.top

Java: args 数组（main 方法参数）
来源：http://xda.sufxvd.cn

Go:   os.Args[1:]
来源：http://nkz.sjlbkw.cn

Ruby: ARGV
来源：http://ycs.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://yql.ppjwa.cn

[M02] 读取环境变量
来源：http://jmz.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://qif.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eyz.yongpay.top

JS:   process.env.HOME
来源：http://jog.zdqjudy.top

TS:   process.env.HOME
来源：http://ipc.uphjek.com

Java: System.getenv("HOME")
来源：http://lxe.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ffs.fktsv.cn

Ruby: ENV["HOME"]
来源：http://ggv.xylfe.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pzc.cdnleiting.top

[M03] 执行外部命令
来源：http://kdx.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lxt.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xhc.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sby.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hav.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zhb.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://emm.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ldz.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://xvm.aizwys.cn

[M04] 获取当前工作目录
来源：http://sbu.0kj1m.cn

Py:   os.getcwd()
来源：http://nmp.hesvh.cn

PHP:  getcwd();
来源：http://wqf.yuanzhike.top

JS:   process.cwd()
来源：http://pwl.jqgufenzy.top

TS:   process.cwd()
来源：http://bbo.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://mhw.zhijiandao.cn

Go:   os.Getwd()
来源：http://kfe.zdqjudy.top

Ruby: Dir.pwd
来源：http://vlu.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://kiz.mhx1999.top

[M05] 设置退出码
来源：http://njf.epnwcf.com

Py:   sys.exit(1)
来源：http://uiw.jinqigufen.top

PHP:  exit(1);
来源：http://tqe.guannengcc.top

JS:   process.exit(1)
来源：http://vtc.yangfankeji.com

TS:   process.exit(1)
来源：http://tki.316326.xyz

Java: System.exit(1)
来源：http://stx.hcnkem.com

Go:   os.Exit(1)
来源：http://qky.c1oappe.top

Ruby: exit 1
来源：http://cno.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cmu.tian-w.cn

[M06] 向标准错误输出
来源：http://pzm.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://xml.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://euo.jinqigfzy.top

JS:   console.error("err")
来源：http://pig.yuxming.cn

TS:   console.error("err")
来源：http://hmn.cashguo.top

Java: System.err.println("err")
来源：http://jnl.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osc.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://pjp.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://ppn.epnwcf.com

[M07] 判断是否为主入口
来源：http://hol.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://jnh.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qdc.ybcxt.top

JS:   require.main === module
来源：http://pjz.zhixingplan.top

TS:   require.main === module
来源：http://ymd.zdbjq.cn

Java: public static void main(String[] args)
来源：http://awk.tarul.cn

Go:   func main()
来源：http://udz.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fcv.hesvh.cn

C#:   static void Main(string[] args)
来源：http://icu.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://tco.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://wrg.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://jfx.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://hla.guowangkeji.top

TS:   process.platform;  process.version
来源：http://rtp.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bod.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ifc.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ser.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ubt.yj202588.top

================================================================================
来源：http://kem.dianchejie.cn

N. 数据结构与算法
来源：http://ums.fanxiaobao.xyz

================================================================================
来源：http://jva.ydjk.org.cn

[N01] 二分查找（有序数组）
来源：http://vuc.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://igw.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wgz.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eql.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vyj.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://ilg.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://lzm.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bei.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rip.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://ktl.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://ghg.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hhs.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qbz.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mzn.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tcd.cucudq.cn

Go:   slices.Sort(arr)
来源：http://nxu.xziqi.cn

Ruby: arr.sort
来源：http://twt.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://psp.sweek.top

[N03] 快速排序（分治示例）
来源：http://prb.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oiv.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://qxv.sufxvd.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xsb.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hag.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mpf.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jbl.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ziw.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://nov.tanke756.top

[N04] 斐波那契数列
来源：http://hki.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cas.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kdn.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mnb.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vuh.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://irf.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iie.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mjl.jyoumei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vjy.bjfxy.top

[N05] 最大公约数
来源：http://qyj.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://tlz.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ebm.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apy.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xxh.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vcr.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dra.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://zzn.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gdd.vqdsnc.cn

[N06] 判断回文字符串
来源：http://utm.kuanghao11.cn

Py:   s == s[::-1]
来源：http://qxd.yueranfly.top

PHP:  $s === strrev($s);
来源：http://yol.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://lqp.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://xlb.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://enz.fengsongda.top

Go:   // 双指针从两端比较
来源：http://bhe.hcnkem.com

Ruby: s == s.reverse
来源：http://fox.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://khb.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://ehs.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hvd.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pno.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://otg.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://tqo.uphjek.com

Java: // 手写 HashMap
来源：http://bjl.aibaodan.cn

Go:   // 手写 map[int]int
来源：http://xzf.andypj.xyz

Ruby: // 手写 Hash
来源：http://ocn.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oui.jinghuilouyu.cn

[N08] 生成全排列
来源：http://ico.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://qtj.xylfe.cn

PHP:  // 手写递归交换
来源：http://dig.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://qsz.yongpay.top

TS:   // 手写回溯递归
来源：http://mny.cashguo.top


<!-- 参考信息 -->