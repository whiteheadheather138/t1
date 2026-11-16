代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://uob.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rrv.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://htg.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baj.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lqj.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://odw.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cmg.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwo.guowangkeji.top

================================================================================
来源：http://zog.meibo888.top

K. JSON 与序列化
来源：http://psg.wangdashe.top

================================================================================
来源：http://dni.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://hli.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qbo.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lze.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://yqa.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://dzl.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cea.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://mcf.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://eto.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xgy.guannengcc.top

[K02] JSON 字符串转对象
来源：http://sps.zhongyouzk.top

Py:   json.loads(s)
来源：http://qrv.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xvm.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://gmj.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://iet.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fex.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://uxr.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://cwz.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kgl.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://tbl.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://muz.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wum.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://szi.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wup.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hmf.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wjn.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uxc.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mfu.fktsv.cn

[K04] 读取 JSON 文件
来源：http://gbw.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://khn.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uug.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kzb.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://akk.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hph.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fkw.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://uqr.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvd.cucudq.cn

[K05] 深拷贝对象
来源：http://qzz.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://ept.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://ast.yueranfly.top

JS:   structuredClone(obj)
来源：http://xvv.hnqzz.top

TS:   structuredClone(obj)
来源：http://xfj.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zjy.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yuw.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vzi.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kci.yj202588.top

[K06] 解析 URL 查询串
来源：http://mpg.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nei.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wig.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smu.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://awp.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gha.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cya.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mxd.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hiz.tianlin.xyz

[K07] 进制转换
来源：http://xwp.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jyh.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rky.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fmv.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lcn.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tse.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tfc.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://som.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oee.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://oql.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://yxn.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dsz.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://hop.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://qde.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fnh.tian-w.cn

Go:   encoding/gob
来源：http://zbu.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://krn.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kil.c1oappe.top

================================================================================
来源：http://axa.yfazqb.com

L. 网络请求
来源：http://kxa.vqdsnc.cn

================================================================================
来源：http://vur.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://aaj.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tbd.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bmb.hongshengwenyu.top

JS:   await fetch(url)
来源：http://otk.hesvh.cn

TS:   await fetch(url)
来源：http://nnm.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ods.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://qwe.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://zfx.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jwu.cdnleiting.top

[L02] 发送 POST JSON
来源：http://ewo.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://ucd.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lxv.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mlv.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bxs.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uwi.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aie.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mjl.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cdh.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://uox.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sft.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dtn.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rkt.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://prq.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://top.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://srb.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://psa.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lup.sweek.top

[L04] 设置超时
来源：http://wry.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://shr.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vzm.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aor.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkt.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://myt.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gmg.yj202588.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://auf.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zpo.yuxming.cn

[L05] 上传文件（multipart）
来源：http://zdn.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kly.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jmd.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wey.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vhc.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://esu.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eot.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aiz.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pop.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://guf.sxryk.cn

Py:   resp.json()
来源：http://wtm.daria6918.cn

PHP:  json_decode($body, true);
来源：http://vfs.hongshengwenyu.top

JS:   await resp.json()
来源：http://dvk.yj20258.top

TS:   await resp.json()
来源：http://wvx.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nco.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ntu.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://ocn.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jhx.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://qnk.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vny.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ran.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://nyl.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://xqh.yonumen.top

Java: resp.statusCode()
来源：http://npa.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://pwh.52xcode.cn

Ruby: resp.code.to_i
来源：http://swi.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://ceu.yfazqb.com

[L08] 并发请求多个地址
来源：http://ezx.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fmp.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://pec.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://akq.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bfg.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kky.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yem.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qec.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rkr.jiagoushi.top

================================================================================
来源：http://uuq.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://uqe.tarul.cn

================================================================================
来源：http://ebr.zhixingplan.top

[M01] 读取命令行参数
来源：http://jiw.316326.xyz

Py:   sys.argv[1:]
来源：http://fju.andypj.xyz

PHP:  $argv;  $argc;
来源：http://iwl.epnwcf.com

JS:   process.argv.slice(2)
来源：http://ogh.xziqi.cn

TS:   process.argv.slice(2)
来源：http://ldp.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://elb.daxiang520.top

Go:   os.Args[1:]
来源：http://iig.uphjek.com

Ruby: ARGV
来源：http://dqo.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://ede.gogol.net.cn

[M02] 读取环境变量
来源：http://yfd.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://jcq.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dyh.kuanghao11.cn

JS:   process.env.HOME
来源：http://fgk.zhijiandao.cn

TS:   process.env.HOME
来源：http://cwp.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://vcg.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ohn.andypj.xyz

Ruby: ENV["HOME"]
来源：http://pjh.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gqq.cheryme.top

[M03] 执行外部命令
来源：http://njx.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kav.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ixd.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zkg.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lna.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iqr.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bcu.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://mzo.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://vcg.fktsv.cn

[M04] 获取当前工作目录
来源：http://dui.sxryk.cn

Py:   os.getcwd()
来源：http://fex.ctjpmb.com

PHP:  getcwd();
来源：http://uku.andypj.xyz

JS:   process.cwd()
来源：http://bxk.yangfankeji.com

TS:   process.cwd()
来源：http://vap.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://rzj.kuanghao11.cn

Go:   os.Getwd()
来源：http://mjq.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://yrs.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oao.zhijiandao.cn

[M05] 设置退出码
来源：http://kvb.hesvh.cn

Py:   sys.exit(1)
来源：http://lpq.gogol.net.cn

PHP:  exit(1);
来源：http://mgf.chenlongwang.top

JS:   process.exit(1)
来源：http://ohy.zhongyouzk.top

TS:   process.exit(1)
来源：http://pax.vehdjk.com

Java: System.exit(1)
来源：http://fkx.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://lfg.daria6918.cn

Ruby: exit 1
来源：http://bzs.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://obp.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://fwg.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://boe.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bko.smart0.xyz

JS:   console.error("err")
来源：http://tvz.shanyushiyangtech.top

TS:   console.error("err")
来源：http://jno.haohaochexian.top

Java: System.err.println("err")
来源：http://mfm.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cnm.vehdjk.com

Ruby: warn "err"
来源：http://aku.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://jxf.guowangkeji.top

[M07] 判断是否为主入口
来源：http://ukw.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://qex.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://get.ppjwa.cn

JS:   require.main === module
来源：http://etc.sjlbkw.cn

TS:   require.main === module
来源：http://yuj.fktsv.cn

Java: public static void main(String[] args)
来源：http://qcf.xuetiantiany.cn

Go:   func main()
来源：http://azs.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://clu.tian-w.cn

C#:   static void Main(string[] args)
来源：http://zjw.sweek.top

[M08] 获取系统与运行时信息
来源：http://fru.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://mfd.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://oju.yuxming.cn

JS:   process.platform;  process.version
来源：http://bwo.yangfankeji.com

TS:   process.platform;  process.version
来源：http://uwy.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vmn.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wph.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://edj.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uim.quarkkingdee.top

================================================================================
来源：http://stt.jiagoushi.top

N. 数据结构与算法
来源：http://wis.cashguo.top

================================================================================
来源：http://cvd.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://ngt.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://fqw.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ury.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sab.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gtu.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://imc.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://jft.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mmp.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://rzf.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://xvm.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://lzq.xuanzx.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mjq.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cza.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ssn.xuanzx.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gqy.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://cfh.fehbvm.com

Ruby: arr.sort
来源：http://wgn.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hzt.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://gxi.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oew.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://eob.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xzg.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tav.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uvm.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vni.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tca.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://odf.yfazqb.com

[N04] 斐波那契数列
来源：http://hyo.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wrq.hesvh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yag.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://myp.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnj.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kyv.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bpu.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://txz.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://awk.xinyue.icu

[N05] 最大公约数
来源：http://ijy.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://aiw.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bkc.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvz.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ysh.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rgu.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tiv.cdnleiting.top

Ruby: a.gcd(b)
来源：http://zjw.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xqn.nanxinkj.top

[N06] 判断回文字符串
来源：http://say.aizwys.cn

Py:   s == s[::-1]
来源：http://tkz.gzhubu.top

PHP:  $s === strrev($s);
来源：http://zhq.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://ulm.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://ifq.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xbl.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://zgk.hesvh.cn

Ruby: s == s.reverse
来源：http://iel.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tlt.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://nmo.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ewz.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sos.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://glz.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://ums.jqgfzy.top

Java: // 手写 HashMap
来源：http://chb.yj202588.top

Go:   // 手写 map[int]int
来源：http://wst.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://zui.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://vlz.c1oappe.top

[N08] 生成全排列
来源：http://qwj.ivvv.top


<!-- 参考信息 -->