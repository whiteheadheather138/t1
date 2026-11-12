代发 wailian999

[G10] 访问控制
来源：http://yqt.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://tld.smart0.xyz

PHP:  public / protected / private
来源：http://pkr.zycfv.cn

JS:   #private 字段；其余公开
来源：http://jyj.c1oappe.top

TS:   public / protected / private
来源：http://ddy.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://mdy.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ees.sufxvd.cn

Ruby: public / protected / private
来源：http://knr.nwbrower.top

C#:   public / protected / private / internal
来源：http://lgk.smart0.xyz

[G11] getter / setter
来源：http://bun.mhx1999.top

Py:   @property 与 @x.setter
来源：http://cik.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xqq.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://kyc.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://amd.andypj.xyz

Java: public String getName() { return name; }
来源：http://hpy.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rlj.fengsongda.top

Ruby: attr_accessor :name
来源：http://tes.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://rfe.gzhubu.top

[G12] 对象转字符串
来源：http://auc.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://vig.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://eut.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://gjb.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://gwt.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://akc.epnwcf.com

Go:   func (u User) String() string { return u.Name }
来源：http://qwe.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://gio.cheryme.top

C#:   public override string ToString() => Name;
来源：http://kpp.hnqzz.top

[G13] 判断对象类型
来源：http://zed.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://mhk.hesvh.cn

PHP:  $u instanceof User
来源：http://hev.ppjwa.cn

JS:   u instanceof User
来源：http://ejc.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://jom.tarul.cn

Java: u instanceof User
来源：http://iqp.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oit.aizwys.cn

Ruby: u.is_a?(User)
来源：http://oia.ydzc1.top

C#:   u is User
来源：http://zzg.iojbl.cn

[G14] 数据类 / record
来源：http://yff.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://meo.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://aej.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://rga.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://uhi.epnwcf.com

Java: record User(String name, int age) {}
来源：http://kem.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://rcn.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://umj.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://lfq.316326.xyz

[G15] 枚举
来源：http://wmj.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://obv.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lbh.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bpl.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fjv.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://kqh.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://net.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://ogm.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pyf.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://pwo.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xsv.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://lze.yangfankeji.com

JS:   Object.entries(obj)
来源：http://stj.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://rxz.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ahx.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jic.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://qrd.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://zgc.jinqigufen.top

================================================================================
来源：http://anj.yvedp.cn

H. 异常与错误处理
来源：http://qjf.chenlongwang.top

================================================================================
来源：http://oxx.quarkkingdee.top

[H01] try / catch 基础
来源：http://snw.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gxk.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dhr.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qpr.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hyp.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cvp.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dij.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fpg.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hzk.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://tlj.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fdy.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://aas.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hkc.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mof.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://wbi.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ucm.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hyj.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tsz.nanxinkj.top

[H03] 主动抛出异常
来源：http://lyp.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://qpt.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yuv.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://wua.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://vmr.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qlg.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lwt.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xga.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://rzc.yuanzhike.top

[H04] 自定义异常类型
来源：http://zbb.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://lux.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://bul.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://vgw.pycfn.com

TS:   class MyError extends Error {}
来源：http://rph.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://mll.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pyu.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://jjs.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://wvd.tarul.cn

[H05] 捕获特定类型
来源：http://dvm.dianchejie.cn

Py:   except ValueError as e:
来源：http://alm.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tjx.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://anw.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://evt.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://lsn.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jfn.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://fjg.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mgz.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://tfz.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://frn.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wgp.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lhd.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://dwk.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eof.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oia.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://cct.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://fkr.ydzc1.top

[H07] 断言
来源：http://tyd.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://zll.cdnleiting.top

PHP:  assert($x > 0);
来源：http://ywn.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://zdz.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://chn.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://dkp.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eyh.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://abt.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://bar.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://gwt.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://mqt.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jdw.316326.xyz

JS:   e.message;  e.stack
来源：http://qod.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://aob.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vus.iojbl.cn

Go:   err.Error()
来源：http://mjz.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://ngv.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://rvi.0kj1m.cn

[H09] 带错误码的异常
来源：http://xut.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kdb.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://dhu.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cis.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://quy.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xpv.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://syx.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://yed.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://jjz.cashguo.top

[H10] 资源自动释放
来源：http://cag.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tas.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rtq.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hpp.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uzg.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wmn.yuanzhike.top

Go:   defer f.Close()
来源：http://rez.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yqd.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pmp.sweek.top

================================================================================
来源：http://nps.c1oappe.top

I. 正则表达式
来源：http://qvg.gogol.net.cn

================================================================================
来源：http://prm.wangdashe.top

[I01] 判断是否匹配
来源：http://kyh.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cfs.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://dyy.jianghu66.top

JS:   /\d+/.test(s)
来源：http://law.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://rgg.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fnh.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bfi.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://jnz.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hpu.andypj.xyz

[I02] 提取所有匹配
来源：http://ite.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://oqq.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ncr.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xjq.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://cax.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gcu.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wgt.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://msd.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wuv.xinyue.icu

[I03] 提取捕获分组
来源：http://xxd.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yuu.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lwo.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ogs.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tux.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zvh.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pvy.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kcq.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://scn.nanxinkj.top

[I04] 正则替换
来源：http://xzf.shuidangran.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mze.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mmr.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oxn.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://tpy.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://qhf.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nrk.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ubi.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dtm.ppjwa.cn

[I05] 按正则拆分
来源：http://odf.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sgh.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fsh.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://quc.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://iee.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://osv.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fvj.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yww.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dyo.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://caj.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://myn.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vyt.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhm.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lxu.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vyg.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mme.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qji.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ntd.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://zmj.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vdt.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sgt.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jiy.sweek.top

TS:   /error/gim
来源：http://xrt.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uzh.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ilx.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://yfv.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://udt.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://foi.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fpz.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vcy.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vji.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gdk.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gom.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yyd.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ltv.ctjpmb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mvx.tarul.cn

================================================================================
来源：http://eci.redwolf501.top

J. 日期与时间
来源：http://qxf.wangshuangyany.cn

================================================================================
来源：http://mgi.ydzc1.top

[J01] 获取当前时间
来源：http://khy.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://psd.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://okl.yueranfly.top

JS:   new Date();  Date.now()
来源：http://hhb.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://sow.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rip.gogol.net.cn

Go:   time.Now()
来源：http://lau.vehdjk.com

Ruby: Time.now
来源：http://xyl.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://efw.kuanghao11.cn

[J02] 格式化输出
来源：http://xbv.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://euo.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bgm.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uct.nanxinkj.top

TS:   d.toISOString()
来源：http://mvm.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gmc.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qtq.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ons.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ngx.dashuyun.cn

[J03] 字符串解析为日期
来源：http://bgq.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nxq.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rju.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://dyr.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://mhw.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://syn.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rsj.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://xwk.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ezj.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://bii.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://orx.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pwd.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dbs.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://vjp.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mvn.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bec.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvo.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tbh.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://hry.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://fbx.hfpthk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bou.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dag.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sec.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://odg.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rwd.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://tjg.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://rec.gotoacloud.top

[J06] 计算两时间之差
来源：http://eou.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://cmc.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://wvv.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yyq.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://doq.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://ldu.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://ehi.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://zvv.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://ecl.snrcjt.cn

[J07] 比较两个日期
来源：http://mmz.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://rdb.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nku.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://ohz.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://zwa.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ven.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aau.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://xhp.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://bzc.daxiang520.top

[J08] 提取年月日与星期
来源：http://rkp.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iio.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vgp.sjlbkw.cn


<!-- 参考信息 -->