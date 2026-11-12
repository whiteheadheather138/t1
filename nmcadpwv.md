代发 wailian999

ROLLBACK TO sp1;
来源：http://khq.xylfe.cn

[Q69] 查看执行计划
来源：http://nkf.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gsd.jinqigufen.top

[Q70] 更新统计信息
来源：http://chf.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://loe.tianlin.xyz

[Q71] 查看建表语句
来源：http://sle.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nop.snrcjt.cn

[Q72] 查看索引
来源：http://niw.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://dyr.jiagoushi.top

[Q73] 查看表状态
来源：http://ftg.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qqo.yongpay.top

[Q74] 强制使用索引
来源：http://uzo.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://guu.cashguo.top

[Q75] 日期格式化
来源：http://aqq.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cjb.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dwp.9152youxi.cn

[Q76] 按天统计
来源：http://prd.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ajy.nanxuanxn.top

[Q77] 时间加减
来源：http://mct.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tul.ivvv.top

[Q78] 当前时间
来源：http://ica.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mmf.snrcjt.cn

[Q79] 字符串拼接
来源：http://pek.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kxm.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://jks.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qno.cheryme.top

[Q81] 字符串替换
来源：http://wzf.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wcm.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://ddz.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wvq.redwolf501.top

[Q83] 大小写转换
来源：http://bvz.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bfh.daxiang520.top

[Q84] 去除首尾空格
来源：http://ell.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://ant.hysaishi.cn

[Q85] 数值取整
来源：http://hpo.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pfi.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://cni.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rki.bjfxy.top

[Q87] JSON 字段做条件
来源：http://xau.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ote.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://qec.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ibn.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zou.ydzc1.top

[Q89] 判断表是否存在
来源：http://nas.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fgm.zdqjudy.top

[Q90] 生成序号列
来源：http://tes.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rab.sxryk.cn

================================================================================
来源：http://dpq.0kj1m.cn

R. Bash 专题
来源：http://tms.tarul.cn

================================================================================
来源：http://asi.cashguo.top

[R01] shebang 与严格模式
来源：http://khx.xziqi.cn

#!/usr/bin/env bash
来源：http://vgu.ctjpmb.com

set -euo pipefail
来源：http://hva.hesvh.cn

[R02] 变量赋值与使用
来源：http://uim.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://mbx.tianlin.xyz

[R03] 只读变量
来源：http://vlo.zhoulong.xyz

readonly PI=3.14
来源：http://wkr.xuanzx.com

[R04] 位置参数
来源：http://url.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jst.sysykeji.top

[R05] 参数默认值
来源：http://vwj.hywenlv.cn

name="${1:-default}"
来源：http://zze.haohaochexian.top

[R06] 判断命令是否存在
来源：http://wls.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vie.jlsjyb.cn

[R07] if 判断文件
来源：http://kep.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ker.pengpengdd.cyou

[R08] 数值比较
来源：http://nzi.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ksb.fktsv.cn

[R09] 字符串比较
来源：http://val.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cqw.zhijiandao.cn

[R10] 正则匹配
来源：http://lok.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vvv.iojbl.cn

[R11] case 多分支
来源：http://nty.vehdjk.com

case "$1" in
来源：http://fqh.aibaodan.cn

start) echo "启动" ;;
来源：http://mhr.wangdashe.top

stop)  echo "停止" ;;
来源：http://orf.cucudq.cn

*)     echo "未知命令" ;;
来源：http://pbz.shanyushiyangkeji.top

esac
来源：http://eir.cheryme.top

[R12] for 遍历文件
来源：http://ydc.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://jmo.quarkkingdee.top

[R13] for 计数循环
来源：http://lse.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://vfz.yfazqb.com

[R14] C 风格 for
来源：http://gri.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wjg.fengsongda.top

[R15] while 逐行读文件
来源：http://boe.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lrq.wangdashe.top

[R16] until 等待条件
来源：http://rba.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zph.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://igc.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://bdo.yvedp.cn

[R18] 遍历数组
来源：http://uja.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vzx.ybcxt.top

[R19] 数组长度
来源：http://mdb.vehdjk.com

echo "${#arr[@]}"
来源：http://bzw.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://zdo.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iua.aizwys.cn

[R21] 字符串长度
来源：http://dqg.xuanzx.com

echo "${#s}"
来源：http://hgi.sysykeji.top

[R22] 截取子串
来源：http://qqo.epnwcf.com

echo "${s:0:5}"
来源：http://nls.cqqwz.cn

[R23] 字符串替换
来源：http://dvm.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hoy.gogol.net.cn

[R24] 大小写转换
来源：http://mim.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://mdm.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://eed.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vmi.yj20258888.top

[R26] 命令替换
来源：http://pgb.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://uxh.jinqigfzy.top

[R27] 算术展开
来源：http://mye.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://non.birdmap.top

[R28] 浮点运算
来源：http://xpb.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://dyz.kuanghao11.cn

[R29] 定义函数
来源：http://nzk.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nmr.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://jul.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://xgt.ctjpmb.com

[R31] 局部变量
来源：http://lmr.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://ljd.bbcook.cn

[R32] 参数个数校验
来源：http://txc.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zzw.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://clo.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lck.cdnleiting.top

[R34] 退出时清理
来源：http://nhj.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bsa.shuidangran.top

[R35] 后台执行并等待
来源：http://zau.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rgw.havefunace.top

[R36] 并发执行多个任务
来源：http://plk.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ddw.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://noh.smart0.xyz

files=$(ls -1)
来源：http://ejp.cheryme.top

[R38] 管道串联
来源：http://tsr.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://ott.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://jvu.svipenyu.cn

cmd > out.log 2>&1
来源：http://zhf.yuxming.cn

[R40] 追加写日志
来源：http://jno.nanxinkj.top

echo "log" >> out.log
来源：http://cnj.havefunace.top

[R41] 丢弃输出
来源：http://baj.uphjek.com

cmd >/dev/null 2>&1
来源：http://yfn.zdbjq.cn

[R42] 输入重定向
来源：http://esa.birdmap.top

wc -l < a.txt
来源：http://jls.fehbvm.com

[R43] 按名字查找文件
来源：http://tbs.tianlin.xyz

find . -name "*.log" -type f
来源：http://scr.guannengcc.top

[R44] 按修改时间查找
来源：http://njp.yangfankeji.com

find . -mtime -7 -type f
来源：http://eiw.iojbl.cn

[R45] 批量删除
来源：http://qun.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://llv.hcnkem.com

[R46] 递归替换文件内容
来源：http://oct.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iwr.yuanzhike.top

[R47] sed 单行替换
来源：http://fsv.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://enj.shangyingyoupin.top

[R48] awk 取指定列
来源：http://zfx.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://sho.tarul.cn

[R49] awk 带条件
来源：http://tva.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xxn.dashuyun.cn

[R50] awk 求和
来源：http://uqt.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zmj.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://ygb.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fcl.zhijiandao.cn

[R52] 统计行数
来源：http://oqg.c1oappe.top

wc -l a.txt
来源：http://xvn.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://kcr.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hdj.fzhhl.top

[R54] 比较两个文件
来源：http://dxq.zhengqikj.top

diff a.txt b.txt
来源：http://lft.quarkkingdee.top

[R55] 压缩与解压
来源：http://fdt.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://igr.yonumen.top

[R56] 远程拷贝
来源：http://jjv.jyoumei.cn

scp file user@host:/path/
来源：http://ifg.feifeiyinyue.top

[R57] 远程执行命令
来源：http://fmw.yj202588.top

ssh user@host 'uptime'
来源：http://mnf.feifeiyinyue.top

[R58] 下载文件
来源：http://vtm.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mdt.gaohongyu789.top

[R59] 发 POST JSON
来源：http://pru.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qcj.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://dcf.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tvt.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://dvt.52xcode.cn

df -h;  du -sh *
来源：http://wql.cucudq.cn

[R62] 找最占空间的文件
来源：http://lpn.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://isw.shangyingyoupin.top

[R63] 内存与进程
来源：http://zgk.uphjek.com

free -h;  ps aux | grep nginx
来源：http://rma.sufxvd.cn

[R64] 结束进程
来源：http://fta.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://zur.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://sdu.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hqw.sysykeji.top

[R66] 定时任务
来源：http://rfk.sxryk.cn

crontab -e;  crontab -l
来源：http://agi.yvedp.cn

[R67] 生成随机十六进制串
来源：http://avh.cqqwz.cn

openssl rand -hex 16
来源：http://qfn.cashguo.top

[R68] 计算文件校验值
来源：http://xwo.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zcs.xuanzx.com

[R69] 生成随机密码
来源：http://zad.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://uzf.chenzaomai.com

[R70] 时间戳与互转
来源：http://zlf.nwbrower.top

date +%s;  date -d @1700000000
来源：http://sei.nwbrower.top

[R71] 日期格式化
来源：http://gwd.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rpj.ydjk.org.cn

[R72] 等待端口就绪
来源：http://rmo.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yjf.yangfankeji.com

[R73] 分割大日志
来源：http://guw.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://obn.gotoacloud.top

[R74] 批量重命名
来源：http://pkz.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dxz.yongpay.top

[R75] 导出环境变量
来源：http://dzf.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://kcb.yonumen.top

[R76] 使用临时文件
来源：http://dlz.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hcx.vehdjk.com

[R77] 读取用户输入
来源：http://ruy.havefunace.top

read -rp "请输入: " ans
来源：http://yap.yj20258.top

[R78] 交互式菜单
来源：http://sdh.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fyk.redwolf501.top

[R79] 解析命令行选项
来源：http://ykr.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vgb.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://toi.svipenyu.cn

time ./run.sh
来源：http://xwp.cdnleiting.top

================================================================================
来源：http://vhp.hywenlv.cn

S. C / C++ 专题
来源：http://ggy.hfpthk.cn

================================================================================
来源：http://nvt.cdnleiting.top

[S01] C：Hello World
来源：http://aoc.ybcxt.top

#include <stdio.h>
来源：http://snj.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qei.sysykeji.top

[S02] C：变量与格式化输出
来源：http://grj.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://vky.xylfe.cn

[S03] C：读入整数
来源：http://zhu.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://rsb.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://mhx.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://rcn.hongshengwenyu.top

[S05] C：字符串长度
来源：http://cyz.pycfn.com

strlen(s)
来源：http://ehi.c1oappe.top

[S06] C：字符串比较
来源：http://kel.yanxiufei.cn

strcmp(a, b) == 0
来源：http://kvu.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://bir.vehdjk.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gjk.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://tsl.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dmj.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://erc.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tcb.xuanzx.com

[S10] C：指针与解引用
来源：http://gwx.cheryme.top

int *p = &a;  *p = 5;
来源：http://ugd.316326.xyz

[S11] C：逐行读文件
来源：http://acz.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://irm.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lyg.yuxming.cn

fclose(f);
来源：http://ydi.jyoumei.cn

[S12] C：写文件
来源：http://hud.jiagoushi.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gfv.andypj.xyz

[S13] C：宏定义
来源：http://hzx.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qlw.zdqjudy.top

[S14] C：枚举
来源：http://bfu.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://csz.316326.xyz

[S15] C：类型转换
来源：http://itw.ybcxt.top

(double) a / b
来源：http://gdj.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://bzw.yonumen.top

x |= (1 << 3);
来源：http://eyz.yonumen.top

[S17] C：安全拼接字符串
来源：http://sst.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yew.xziqi.cn

[S18] C：命令行参数
来源：http://ngf.pycfn.com

int main(int argc, char **argv)
来源：http://ueq.jlsjyb.cn

[S19] C：快速排序
来源：http://xpl.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://mck.shuidangran.top

[S20] C：二分查找
来源：http://rwh.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ouv.yvedp.cn

[S21] C：字符类别判断
来源：http://sjx.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://frs.xuanzx.com

[S22] C：字符串转数字
来源：http://zhb.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://mom.gotoacloud.top

[S23] C：随机数
来源：http://hpv.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jua.hnqzz.top

[S24] C：获取本地时间
来源：http://fqv.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uat.jianghu66.top

[S25] C：内存拷贝
来源：http://wpk.jianghu66.top

memcpy(dst, src, n);
来源：http://cmh.zhengqikj.top

[S26] C：内存清零
来源：http://asz.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://qhi.zhixingplan.top

[S27] C：定义常量
来源：http://wco.gotoacloud.top

const double PI = 3.14159;
来源：http://qjz.yj202588.top

[S28] C：静态变量
来源：http://kyc.fengsongda.top

static int counter = 0;
来源：http://hry.guannengcc.top

[S29] C：变参函数
来源：http://xqv.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://unw.jiagoushi.top

[S30] C：头文件保护
来源：http://gzz.bbcook.cn

#ifndef X_H
来源：http://zln.xingfuxueyuan.xyz

#define X_H
来源：http://viz.yvedp.cn

#endif
来源：http://gxt.gogol.net.cn

[S31] C++：Hello World
来源：http://mld.pycfn.com

#include <iostream>
来源：http://jdh.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://zkn.ctjpmb.com

[S32] C++：字符串
来源：http://swz.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://bnu.quarkkingdee.top

[S33] C++：vector 增删
来源：http://rgb.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://euh.cdnleiting.top

[S34] C++：遍历 vector
来源：http://ryy.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://wuz.shanyushiyangkeji.top

[S35] C++：map
来源：http://rza.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zzl.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://ukl.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pxp.haohaochexian.top

[S37] C++：set
来源：http://syh.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oip.chenjidiqi.icu

[S38] C++：排序
来源：http://raa.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://jxa.jinghuilouyu.cn


<!-- 参考信息 -->