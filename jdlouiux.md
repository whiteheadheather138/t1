代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://czd.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://fwa.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cuf.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pev.jqgfzy.top

[Q76] 按天统计
来源：http://mog.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://knc.pengpengdd.cyou

[Q77] 时间加减
来源：http://awf.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cuq.kuanghao11.cn

[Q78] 当前时间
来源：http://uel.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bya.zycfv.cn

[Q79] 字符串拼接
来源：http://ibw.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tdq.wangdashe.top

[Q80] 字符串截取
来源：http://ukj.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kjd.zhijiandao.cn

[Q81] 字符串替换
来源：http://mse.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rkl.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://wnh.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://adw.zhiwuduotai.top

[Q83] 大小写转换
来源：http://tzk.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vrm.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://eis.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://wby.yuanzhike.top

[Q85] 数值取整
来源：http://vql.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kwf.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://nwd.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zkk.hammf.cn

[Q87] JSON 字段做条件
来源：http://ebp.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://beg.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://sjj.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qup.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rjm.epnwcf.com

[Q89] 判断表是否存在
来源：http://rjf.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ucf.cqqwz.cn

[Q90] 生成序号列
来源：http://fyh.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kcl.redwolf501.top

================================================================================
来源：http://ayt.jinyuanbaomall.cn

R. Bash 专题
来源：http://wsr.nanxuanxn.top

================================================================================
来源：http://lps.zhixingplan.top

[R01] shebang 与严格模式
来源：http://xmd.hysaishi.cn

#!/usr/bin/env bash
来源：http://ywx.zdbjq.cn

set -euo pipefail
来源：http://doy.aizwys.cn

[R02] 变量赋值与使用
来源：http://tqc.tarul.cn

name="Tom"; echo "$name"
来源：http://jxr.tarul.cn

[R03] 只读变量
来源：http://oqi.jinghuilouyu.cn

readonly PI=3.14
来源：http://vwl.haohaochexian.top

[R04] 位置参数
来源：http://vzf.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hdk.haohaochexian.top

[R05] 参数默认值
来源：http://kwo.gzhubu.top

name="${1:-default}"
来源：http://ldq.hammf.cn

[R06] 判断命令是否存在
来源：http://qsj.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uyc.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://fqf.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rwj.hammf.cn

[R08] 数值比较
来源：http://hwm.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dfs.fengsongda.top

[R09] 字符串比较
来源：http://dzq.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hxf.c1oappe.top

[R10] 正则匹配
来源：http://myr.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qak.wangdashe.top

[R11] case 多分支
来源：http://kqc.zhoulong.xyz

case "$1" in
来源：http://sqd.gaohongyu789.top

start) echo "启动" ;;
来源：http://lsu.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://rjd.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://and.xuetiantiany.cn

esac
来源：http://vaw.yvedp.cn

[R12] for 遍历文件
来源：http://xdq.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://kbw.iojbl.cn

[R13] for 计数循环
来源：http://zey.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://dea.andypj.xyz

[R14] C 风格 for
来源：http://qce.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wct.0kj1m.cn

[R15] while 逐行读文件
来源：http://tml.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uyg.jinqigfzy.top

[R16] until 等待条件
来源：http://cpm.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://abg.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://xdd.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jro.jinqigfzy.top

[R18] 遍历数组
来源：http://cvt.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jle.fktsv.cn

[R19] 数组长度
来源：http://gtw.tanke756.top

echo "${#arr[@]}"
来源：http://zsi.hywenlv.cn

[R20] 关联数组（字典）
来源：http://xwt.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cyk.zhongyouzk.top

[R21] 字符串长度
来源：http://uhf.hysaishi.cn

echo "${#s}"
来源：http://vxu.cashguo.top

[R22] 截取子串
来源：http://woa.hnqzz.top

echo "${s:0:5}"
来源：http://fls.epnwcf.com

[R23] 字符串替换
来源：http://kqh.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ovn.xinyue.icu

[R24] 大小写转换
来源：http://zzq.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dol.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://jsh.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://oer.hnxiangtu.top

[R26] 命令替换
来源：http://ztk.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://auw.tian-w.cn

[R27] 算术展开
来源：http://mlf.yuxming.cn

echo $((1 + 2 * 3))
来源：http://dod.birdmap.top

[R28] 浮点运算
来源：http://gow.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://hkz.yanxiufei.cn

[R29] 定义函数
来源：http://jqk.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zma.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://oep.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://sfy.cqqwz.cn

[R31] 局部变量
来源：http://qpj.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://kys.nwbrower.top

[R32] 参数个数校验
来源：http://kxr.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bil.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://yte.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sjz.wangshuangyany.cn

[R34] 退出时清理
来源：http://dfy.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://htj.yangfankeji.com

[R35] 后台执行并等待
来源：http://sgz.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zys.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://pil.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pcy.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://pdi.tanke756.top

files=$(ls -1)
来源：http://ehb.zhaomingkeji.xyz

[R38] 管道串联
来源：http://dnu.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://uko.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://plf.epnwcf.com

cmd > out.log 2>&1
来源：http://rxi.yonumen.top

[R40] 追加写日志
来源：http://wwu.xylfe.cn

echo "log" >> out.log
来源：http://rso.tanke756.top

[R41] 丢弃输出
来源：http://prd.yuxming.cn

cmd >/dev/null 2>&1
来源：http://pfv.chenjidiqi.icu

[R42] 输入重定向
来源：http://gad.tianlin.xyz

wc -l < a.txt
来源：http://obj.yj20258.top

[R43] 按名字查找文件
来源：http://wbw.316326.xyz

find . -name "*.log" -type f
来源：http://ptb.cheryme.top

[R44] 按修改时间查找
来源：http://jyv.guowangkeji.top

find . -mtime -7 -type f
来源：http://slg.yj20258888.top

[R45] 批量删除
来源：http://wgi.tarul.cn

find . -name "*.tmp" -delete
来源：http://vdz.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://fqp.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sbk.redwolf501.top

[R47] sed 单行替换
来源：http://pzy.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://lul.nanxinkj.top

[R48] awk 取指定列
来源：http://mxb.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://aai.cdnleiting.top

[R49] awk 带条件
来源：http://qph.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pjb.zdqjudy.top

[R50] awk 求和
来源：http://bdx.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://coe.bbcook.cn

[R51] 排序去重取前几
来源：http://net.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://thu.yj20258.top

[R52] 统计行数
来源：http://vat.zhixingplan.top

wc -l a.txt
来源：http://cba.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://nmq.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ibq.xuetiantiany.cn

[R54] 比较两个文件
来源：http://xjo.gaohongyu789.top

diff a.txt b.txt
来源：http://fwf.hnqzz.top

[R55] 压缩与解压
来源：http://iii.jinyuanbaomall.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://odh.jiagoushi.top

[R56] 远程拷贝
来源：http://rqb.sufxvd.cn

scp file user@host:/path/
来源：http://zio.ydzc1.top

[R57] 远程执行命令
来源：http://jnk.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://utz.yuxming.cn

[R58] 下载文件
来源：http://gdm.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wsa.gogol.net.cn

[R59] 发 POST JSON
来源：http://mxd.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://doq.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://vrv.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rol.zhixingplan.top

[R61] 磁盘占用
来源：http://dwl.jinqigufen.top

df -h;  du -sh *
来源：http://yrk.aibaodan.cn

[R62] 找最占空间的文件
来源：http://lwr.uphjek.com

du -ah . | sort -rh | head -10
来源：http://cne.fengsongda.top

[R63] 内存与进程
来源：http://egy.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://enz.gogol.net.cn

[R64] 结束进程
来源：http://yui.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://hbu.yj20258.top

[R65] 查看端口占用
来源：http://hqu.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yxn.uphjek.com

[R66] 定时任务
来源：http://jdj.c1oappe.top

crontab -e;  crontab -l
来源：http://fld.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://hqo.jlsjyb.cn

openssl rand -hex 16
来源：http://mhp.pengpengdd.cyou

[R68] 计算文件校验值
来源：http://viu.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://zbv.pengpengdd.cyou

[R69] 生成随机密码
来源：http://bse.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://bmb.uphjek.com

[R70] 时间戳与互转
来源：http://und.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://nan.smart0.xyz

[R71] 日期格式化
来源：http://voi.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://cnr.sjlbkw.cn

[R72] 等待端口就绪
来源：http://fdx.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://uzu.hysaishi.cn

[R73] 分割大日志
来源：http://din.uphjek.com

split -l 1000 big.log part_
来源：http://rox.dianchejie.cn

[R74] 批量重命名
来源：http://uei.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jfa.yuanzhike.top

[R75] 导出环境变量
来源：http://ahp.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://zyv.wangshuangyany.cn

[R76] 使用临时文件
来源：http://npj.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nmn.quarkkingdee.top

[R77] 读取用户输入
来源：http://gqm.vqdsnc.cn

read -rp "请输入: " ans
来源：http://xpd.yj202588.top

[R78] 交互式菜单
来源：http://drs.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://njz.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://ktw.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hun.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://esi.daria6918.cn

time ./run.sh
来源：http://ntt.nanxinkj.top

================================================================================
来源：http://vah.hnqzz.top

S. C / C++ 专题
来源：http://gyv.tarul.cn

================================================================================
来源：http://sgk.pengpengdd.cyou

[S01] C：Hello World
来源：http://umw.mhx1999.top

#include <stdio.h>
来源：http://kjg.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://eso.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://nen.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://bdy.316326.xyz

[S03] C：读入整数
来源：http://oer.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://vyd.andypj.xyz

[S04] C：字符串复制
来源：http://iwm.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://urb.yueranfly.top

[S05] C：字符串长度
来源：http://apl.zhongyouzk.top

strlen(s)
来源：http://dxo.yueranfly.top

[S06] C：字符串比较
来源：http://xlh.shuidangran.top

strcmp(a, b) == 0
来源：http://yht.yueranfly.top

[S07] C：数组遍历求和
来源：http://eav.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zel.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://tiu.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ykp.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://ind.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ndb.ydjk.org.cn

[S10] C：指针与解引用
来源：http://uke.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://puh.vqdsnc.cn

[S11] C：逐行读文件
来源：http://pmi.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://gik.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aun.zhiwuduotai.top

fclose(f);
来源：http://icm.yj202588.top

[S12] C：写文件
来源：http://tjp.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dti.haohaochexian.top

[S13] C：宏定义
来源：http://txg.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kyv.ivvv.top

[S14] C：枚举
来源：http://xad.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://ddf.sjlbkw.cn

[S15] C：类型转换
来源：http://ezv.xingfuxueyuan.xyz

(double) a / b
来源：http://ovt.yvedp.cn

[S16] C：位操作置位
来源：http://xui.aizwys.cn

x |= (1 << 3);
来源：http://fav.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://ahl.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qfg.kuanghao11.cn

[S18] C：命令行参数
来源：http://wit.tanke756.top

int main(int argc, char **argv)
来源：http://wbk.guannengcc.top

[S19] C：快速排序
来源：http://lch.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://hsm.hywenlv.cn

[S20] C：二分查找
来源：http://mac.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oxm.vqdsnc.cn

[S21] C：字符类别判断
来源：http://wrl.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vsm.gaohongyu789.top

[S22] C：字符串转数字
来源：http://rfk.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sgk.redwolf501.top

[S23] C：随机数
来源：http://lnz.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nqr.fzhhl.top

[S24] C：获取本地时间
来源：http://jjs.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ptk.yueranfly.top

[S25] C：内存拷贝
来源：http://ubr.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://fwn.tarul.cn

[S26] C：内存清零
来源：http://dbe.epnwcf.com

memset(a, 0, sizeof a);
来源：http://osh.cdnleiting.top

[S27] C：定义常量
来源：http://ydd.chenzaomai.com

const double PI = 3.14159;
来源：http://oyy.feifeiyinyue.top

[S28] C：静态变量
来源：http://cko.jqgufenzy.top

static int counter = 0;
来源：http://omj.yj20258888.top

[S29] C：变参函数
来源：http://zfj.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nsj.sxryk.cn

[S30] C：头文件保护
来源：http://skb.fanxiaobao.xyz

#ifndef X_H
来源：http://dam.cdnleiting.top

#define X_H
来源：http://goa.fehbvm.com

#endif
来源：http://xee.jyoumei.cn

[S31] C++：Hello World
来源：http://vlt.zhaomingkeji.xyz

#include <iostream>
来源：http://hzk.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://nzz.svipenyu.cn

[S32] C++：字符串
来源：http://dxp.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://lji.yangfankeji.com

[S33] C++：vector 增删
来源：http://xso.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://auy.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://xns.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://ifn.gogol.net.cn

[S35] C++：map
来源：http://lcy.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tah.c1oappe.top

[S36] C++：unordered_map
来源：http://pea.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wur.ydjk.org.cn

[S37] C++：set
来源：http://gfc.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eqm.jinqigfzy.top

[S38] C++：排序
来源：http://cfi.zhongyouzk.top

std::sort(v.begin(), v.end());
来源：http://pln.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://ccs.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zzf.zhiwuduotai.top

[S40] C++：查找元素
来源：http://cjl.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://msw.hcnkem.com

[S41] C++：类与构造函数
来源：http://tzu.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qos.cashguo.top

[S42] C++：继承与虚函数
来源：http://xzb.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://sld.chenzaomai.com

[S43] C++：智能指针
来源：http://qec.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://yga.ydjk.org.cn

[S44] C++：引用传参
来源：http://jqz.c1oappe.top

void inc(int &x) { ++x; }
来源：http://hzw.ywan-chungtsiang.top


<!-- 参考信息 -->