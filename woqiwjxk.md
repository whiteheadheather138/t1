代发 wailian999

Ruby: attr_accessor :name
来源：http://rfq.fktsv.cn

C#:   public string Name { get; set; }
来源：http://noz.andypj.xyz

[G12] 对象转字符串
来源：http://cox.yongpay.top

Py:   def __str__(self): return self.name
来源：http://pzd.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nla.wangdashe.top

JS:   toString() { return this.name; }
来源：http://yxk.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://ymi.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://vdq.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://brq.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://dws.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://svd.fktsv.cn

[G13] 判断对象类型
来源：http://nzo.bjfxy.top

Py:   isinstance(u, User)
来源：http://lis.cqqwz.cn

PHP:  $u instanceof User
来源：http://azs.shangyingyoupin.top

JS:   u instanceof User
来源：http://tol.sufxvd.cn

TS:   u instanceof User
来源：http://uvm.jinqigfzy.top

Java: u instanceof User
来源：http://tou.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://let.sxryk.cn

Ruby: u.is_a?(User)
来源：http://pff.tarul.cn

C#:   u is User
来源：http://ykb.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://cqz.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qhg.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://olo.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dik.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://yxd.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://mcs.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://rpx.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ygl.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://oez.fanxiaobao.xyz

[G15] 枚举
来源：http://vkt.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wqv.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xgl.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zhl.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bbv.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://oud.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lai.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://yzt.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://caq.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://wgy.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pxt.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://jus.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://vbj.epnwcf.com

TS:   Object.entries(obj)
来源：http://afc.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xpe.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://smg.birdmap.top

Ruby: obj.instance_variables
来源：http://fbs.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://bao.ybcxt.top

================================================================================
来源：http://vww.yueranfly.top

H. 异常与错误处理
来源：http://yuf.zycfv.cn

================================================================================
来源：http://nhi.sxryk.cn

[H01] try / catch 基础
来源：http://vgf.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jhq.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ncx.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://spv.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wbp.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oyk.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sbv.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kdf.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mey.smart0.xyz

[H02] finally / ensure 收尾
来源：http://jfz.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uym.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hjn.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://yia.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wfs.ywan-chungtsiang.top

Java: try { f(); } finally { cleanup(); }
来源：http://znc.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ymc.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://afw.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dax.meibo888.top

[H03] 主动抛出异常
来源：http://cmu.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://lqp.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qpv.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://oye.havefunace.top

TS:   throw new Error("错误信息");
来源：http://zes.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aii.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://diw.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qgo.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://mdx.chenlongwang.top

[H04] 自定义异常类型
来源：http://kye.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://jtb.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://zta.tarul.cn

JS:   class MyError extends Error {}
来源：http://cek.xinyue.icu

TS:   class MyError extends Error {}
来源：http://ucw.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://hbr.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vkx.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://vzb.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://mex.yangfankeji.com

[H05] 捕获特定类型
来源：http://cei.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://pmp.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jls.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://zpi.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://pan.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://jqt.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://juw.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://ghi.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wis.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://fjb.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://bsu.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://cly.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://rph.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yeq.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://svj.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nrk.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://oje.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://wtv.zhongyouzk.top

[H07] 断言
来源：http://tvj.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://jun.yangfankeji.com

PHP:  assert($x > 0);
来源：http://lfl.fengsongda.top

JS:   console.assert(x > 0);
来源：http://fkh.tarul.cn

TS:   console.assert(x > 0);
来源：http://jyf.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://lqn.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vtm.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ctv.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://mdb.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://bpg.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://lls.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://arl.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://omm.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ouk.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hck.yj202588.top

Go:   err.Error()
来源：http://wex.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://bfl.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://ymk.9152youxi.cn

[H09] 带错误码的异常
来源：http://knm.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jkp.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eop.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vcy.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jec.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qox.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jdf.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://oln.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rkn.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://quv.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eoe.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fsr.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iww.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vdt.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wzv.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://skn.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ngu.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://grj.zhaomingkeji.xyz

================================================================================
来源：http://wkw.epnwcf.com

I. 正则表达式
来源：http://vcv.chenlongwang.top

================================================================================
来源：http://npm.cucudq.cn

[I01] 判断是否匹配
来源：http://rbe.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eoz.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lsz.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://owa.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://mhz.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yib.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://knd.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://lza.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sug.zycfv.cn

[I02] 提取所有匹配
来源：http://whi.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://xes.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rwc.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qph.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://zda.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wll.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://srn.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://zwa.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oip.pycfn.com

[I03] 提取捕获分组
来源：http://lro.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qwa.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fhw.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vci.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kbv.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lnm.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://btk.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dfs.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xld.yanxiufei.cn

[I04] 正则替换
来源：http://dmv.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gnu.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zzi.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://ycg.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lmc.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://jsq.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dzg.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dba.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tez.jianghu66.top

[I05] 按正则拆分
来源：http://zvi.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://glk.chenjidiqi.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jbe.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://mhf.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://nbl.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://nyj.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bda.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://nvl.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eoc.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vbi.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xby.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mgu.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcl.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tib.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jjd.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hia.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dnw.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yoj.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://nsn.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xdy.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rmy.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://erl.hongshengwenyu.top

TS:   /error/gim
来源：http://gmc.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dxq.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sbq.sweek.top

Ruby: s.scan(/error/i)
来源：http://hoc.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yro.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://tfl.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gqs.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aro.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nsu.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gbe.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://abv.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eev.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rcr.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://asf.yanxiufei.cn

================================================================================
来源：http://nct.xylfe.cn

J. 日期与时间
来源：http://aec.chenlongwang.top

================================================================================
来源：http://eth.xuanzx.com

[J01] 获取当前时间
来源：http://lcq.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ddy.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ipy.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://brr.redwolf501.top

TS:   new Date();  Date.now()
来源：http://kvv.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cat.ehwqpu.com

Go:   time.Now()
来源：http://tac.c1oappe.top

Ruby: Time.now
来源：http://gqw.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://keo.hongshengwenyu.top

[J02] 格式化输出
来源：http://xqc.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xea.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bgt.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yub.nwbrower.top

TS:   d.toISOString()
来源：http://adp.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iyy.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mny.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hok.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rhn.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://xsi.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wlm.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qcy.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://epg.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://krb.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://pdw.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qte.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://sba.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ckz.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://ujz.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nov.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nif.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://skt.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cho.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wey.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rzx.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uhx.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iyx.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://duw.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://avy.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://tqk.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqd.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rqq.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://kjw.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uce.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://ibm.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gzw.smart0.xyz

[J06] 计算两时间之差
来源：http://csj.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://eqq.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://bmd.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tva.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ijj.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://kln.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://aym.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://nsl.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://ajr.pycfn.com

[J07] 比较两个日期
来源：http://kaj.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://erp.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://irt.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://efp.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://atl.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ddg.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://msj.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://nlk.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://iog.fengsongda.top

[J08] 提取年月日与星期
来源：http://agp.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kli.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nqb.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ned.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wsb.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aui.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://end.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ibu.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tbp.jyoumei.cn

[J09] 时区处理
来源：http://ogz.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tyc.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tul.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zat.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kcv.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ohm.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://diz.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hlj.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eyg.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://aeb.fktsv.cn


<!-- 参考信息 -->