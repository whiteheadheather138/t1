代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mgi.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tcd.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fgs.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://giv.fengsongda.top

================================================================================
来源：http://wre.guowangkeji.top

K. JSON 与序列化
来源：http://imb.hfpthk.cn

================================================================================
来源：http://iss.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://ybi.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pes.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ovt.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://ect.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://ocv.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mau.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://unz.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://hna.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://stz.vehdjk.com

[K02] JSON 字符串转对象
来源：http://uop.pycfn.com

Py:   json.loads(s)
来源：http://lph.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://erh.snrcjt.cn

JS:   JSON.parse(s)
来源：http://ojj.cucudq.cn

TS:   JSON.parse(s)
来源：http://tzt.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bed.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://lgf.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://ixa.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uzx.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://gqg.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kyf.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pgg.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ccs.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vnv.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kru.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dof.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hpj.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hmf.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://fzt.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gav.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hhi.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tff.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cep.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qov.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wyc.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://kff.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://krs.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://qyg.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://zpi.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://avx.andypj.xyz

JS:   structuredClone(obj)
来源：http://cpj.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://krr.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ywx.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://erz.yj20258.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qjj.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pre.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://puy.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yfa.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zzx.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vsp.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pjg.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xts.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://djd.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nhp.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wdy.tian-w.cn

[K07] 进制转换
来源：http://zsl.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ixr.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tjn.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lkv.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gwd.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dqc.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eyi.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kwf.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://han.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ost.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://bxm.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vtq.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://emy.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://ktg.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hlt.hesvh.cn

Go:   encoding/gob
来源：http://hdv.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://mpu.ydzc1.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://azi.aizwys.cn

================================================================================
来源：http://tmi.0kj1m.cn

L. 网络请求
来源：http://ojo.zhongyouzk.top

================================================================================
来源：http://cnj.jianghu66.top

[L01] 发送 GET 请求
来源：http://blv.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hzi.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jnv.fehbvm.com

JS:   await fetch(url)
来源：http://bwu.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://okp.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wrh.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://hec.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xca.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://irz.guannengcc.top

[L02] 发送 POST JSON
来源：http://szh.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nke.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vbu.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eoq.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zfx.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kif.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tyo.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rew.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://koo.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://kcj.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jfu.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wvn.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://anh.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ixx.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://imh.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cio.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mpl.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hup.shuidangran.top

[L04] 设置超时
来源：http://mcx.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://cux.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zgd.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfj.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhh.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ysz.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://svw.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rrx.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rhx.bjfxy.top

[L05] 上传文件（multipart）
来源：http://mmd.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vfo.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://epn.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wid.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://azj.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mrr.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wvk.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://roy.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cka.xuanzx.com

[L06] 解析响应为 JSON
来源：http://epd.uphjek.com

Py:   resp.json()
来源：http://mrg.yongpay.top

PHP:  json_decode($body, true);
来源：http://naa.zhijiandao.cn

JS:   await resp.json()
来源：http://ltv.shuidangran.top

TS:   await resp.json()
来源：http://drg.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ual.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cmm.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://gkf.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wod.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://lmr.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eyf.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mjm.tanke756.top

JS:   resp.ok;  resp.status
来源：http://jdk.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://hwt.fzhhl.top

Java: resp.statusCode()
来源：http://cbw.yuxming.cn

Go:   resp.StatusCode
来源：http://khu.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://hmx.pycfn.com

C#:   (int)resp.StatusCode
来源：http://zdm.cqqwz.cn

[L08] 并发请求多个地址
来源：http://mmx.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tiw.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://fan.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bfw.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hnf.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zcr.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kjt.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jnv.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xrs.cucudq.cn

================================================================================
来源：http://jzt.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://lmp.aizwys.cn

================================================================================
来源：http://uhs.yueranfly.top

[M01] 读取命令行参数
来源：http://vup.yonumen.top

Py:   sys.argv[1:]
来源：http://rhb.nwbrower.top

PHP:  $argv;  $argc;
来源：http://kcs.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://ssx.hammf.cn

TS:   process.argv.slice(2)
来源：http://otf.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://hzc.jqgfzy.top

Go:   os.Args[1:]
来源：http://uiw.316326.xyz

Ruby: ARGV
来源：http://pmj.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://kyl.fehbvm.com

[M02] 读取环境变量
来源：http://skj.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://bnk.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ptl.zhoulong.xyz

JS:   process.env.HOME
来源：http://ilw.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://jtk.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://pxr.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vzx.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://xkl.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ytk.havefunace.top

[M03] 执行外部命令
来源：http://jpc.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lsk.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sps.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sld.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bhr.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dvu.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eri.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://vdr.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://yeh.0kj1m.cn

[M04] 获取当前工作目录
来源：http://ugv.gaohongyu789.top

Py:   os.getcwd()
来源：http://eka.redwolf501.top

PHP:  getcwd();
来源：http://qau.yanxiufei.cn

JS:   process.cwd()
来源：http://spg.zhongyouzk.top

TS:   process.cwd()
来源：http://yeb.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://iko.shuidangran.top

Go:   os.Getwd()
来源：http://ptu.quarkkingdee.top

Ruby: Dir.pwd
来源：http://xob.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://fyr.jinqigufen.top

[M05] 设置退出码
来源：http://jco.c1oappe.top

Py:   sys.exit(1)
来源：http://yxl.nwbrower.top

PHP:  exit(1);
来源：http://inx.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://zht.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://xrl.zdqjudy.top

Java: System.exit(1)
来源：http://bwr.daxiang520.top

Go:   os.Exit(1)
来源：http://dax.yongpay.top

Ruby: exit 1
来源：http://pmw.ywan-chungtsiang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ydh.bjfxy.top

[M06] 向标准错误输出
来源：http://vue.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://lae.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://znn.jyoumei.cn

JS:   console.error("err")
来源：http://mwm.9152youxi.cn

TS:   console.error("err")
来源：http://ose.jyoumei.cn

Java: System.err.println("err")
来源：http://jnv.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://afz.pycfn.com

Ruby: warn "err"
来源：http://sgc.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://eit.ehwqpu.com

[M07] 判断是否为主入口
来源：http://bxs.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://obn.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vbo.aizwys.cn

JS:   require.main === module
来源：http://qeq.guannengcc.top

TS:   require.main === module
来源：http://yqg.epnwcf.com

Java: public static void main(String[] args)
来源：http://tzn.shuidangran.top

Go:   func main()
来源：http://bmr.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gro.hesvh.cn

C#:   static void Main(string[] args)
来源：http://mdo.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://zxr.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://bod.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://cbv.tianlin.xyz

JS:   process.platform;  process.version
来源：http://gfh.tian-w.cn

TS:   process.platform;  process.version
来源：http://zwy.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vww.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xkc.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tcg.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hcs.uphjek.com

================================================================================
来源：http://bzh.andypj.xyz

N. 数据结构与算法
来源：http://chf.cqqwz.cn

================================================================================
来源：http://rlb.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://doq.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://imj.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dzc.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zib.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://inc.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pyh.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://gua.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ptp.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://ebb.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://zuo.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://juk.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nyf.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lbe.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://owa.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gyl.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://wou.chenlongwang.top

Ruby: arr.sort
来源：http://dgh.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://urp.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://dxf.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zkh.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://gaj.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdl.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dfj.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zcp.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ype.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bhd.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://qhd.52xcode.cn

[N04] 斐波那契数列
来源：http://gbu.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uth.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lnm.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hie.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyx.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pzu.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rbk.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xaq.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bew.tian-w.cn

[N05] 最大公约数
来源：http://udd.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://ifk.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lmt.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dhh.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qwu.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hlc.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qri.yj202588.top

Ruby: a.gcd(b)
来源：http://qlm.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sre.shzxlz.cn

[N06] 判断回文字符串
来源：http://jtf.hywenlv.cn

Py:   s == s[::-1]
来源：http://qui.yuxming.cn

PHP:  $s === strrev($s);
来源：http://lma.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://txc.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://sah.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bxm.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://pgi.yfazqb.com

Ruby: s == s.reverse
来源：http://syl.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ufg.yonumen.top

[N07] 两数之和（返回下标）
来源：http://rfr.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tbq.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://siv.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jjh.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://aem.hesvh.cn

Java: // 手写 HashMap
来源：http://yil.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://mxk.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://ixi.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://edc.fktsv.cn

[N08] 生成全排列
来源：http://xvz.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://wkh.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://xeo.fehbvm.com

JS:   // 手写回溯递归
来源：http://ock.shzxlz.cn

TS:   // 手写回溯递归
来源：http://uid.sxryk.cn


<!-- 参考信息 -->