代发 wailian999

[Q61] 移动平均
来源：http://dop.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vuz.andypj.xyz

[Q62] 分组占比
来源：http://tsz.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ymg.birdmap.top

[Q63] 开启事务
来源：http://uxv.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://udh.kuanghao11.cn

[Q64] 提交事务
来源：http://jkz.ctjpmb.com

COMMIT;
来源：http://dtt.mhx1999.top

[Q65] 回滚事务
来源：http://ast.ehwqpu.com

ROLLBACK;
来源：http://zbk.epnwcf.com

[Q66] 行锁查询
来源：http://hfi.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qgk.snrcjt.cn

[Q67] 设置隔离级别
来源：http://aig.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zkf.daxiang520.top

[Q68] 保存点
来源：http://lbu.fehbvm.com

SAVEPOINT sp1;
来源：http://uny.hysaishi.cn

ROLLBACK TO sp1;
来源：http://pvh.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://zxd.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ued.yj202588.top

[Q70] 更新统计信息
来源：http://vvf.ctjpmb.com

ANALYZE TABLE users;
来源：http://bnt.tarul.cn

[Q71] 查看建表语句
来源：http://kxz.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hic.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://mik.daxiang520.top

SHOW INDEX FROM users;
来源：http://cns.cheryme.top

[Q73] 查看表状态
来源：http://wnf.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://azz.chenlongwang.top

[Q74] 强制使用索引
来源：http://ype.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fms.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://isj.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rca.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://htd.ctjpmb.com

[Q76] 按天统计
来源：http://joh.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qcv.c1oappe.top

[Q77] 时间加减
来源：http://kwg.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xup.aibaodan.cn

[Q78] 当前时间
来源：http://snq.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gdr.daxiang520.top

[Q79] 字符串拼接
来源：http://idl.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mxa.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://tyn.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lvv.ydjk.org.cn

[Q81] 字符串替换
来源：http://ggz.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://num.316326.xyz

[Q82] 字符长度与字节长度
来源：http://wpx.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dll.pengpengdd.cyou

[Q83] 大小写转换
来源：http://lbu.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qjz.52xcode.cn

[Q84] 去除首尾空格
来源：http://lav.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://ytj.hnxiangtu.top

[Q85] 数值取整
来源：http://ene.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qsj.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://ebx.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dva.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://ury.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wut.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://rex.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pjf.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rxv.316326.xyz

[Q89] 判断表是否存在
来源：http://jrh.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zka.nanxuanxn.top

[Q90] 生成序号列
来源：http://oey.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mrx.ywan-chungtsiang.top

================================================================================
来源：http://xkd.hfpthk.cn

R. Bash 专题
来源：http://pri.zhongyouzk.top

================================================================================
来源：http://zir.hywenlv.cn

[R01] shebang 与严格模式
来源：http://dik.jinqigufen.top

#!/usr/bin/env bash
来源：http://lmu.mhx1999.top

set -euo pipefail
来源：http://foc.yfazqb.com

[R02] 变量赋值与使用
来源：http://uth.yuxming.cn

name="Tom"; echo "$name"
来源：http://mib.daxiang520.top

[R03] 只读变量
来源：http://gte.zdbjq.cn

readonly PI=3.14
来源：http://mll.chenlongwang.top

[R04] 位置参数
来源：http://aay.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://khn.0kj1m.cn

[R05] 参数默认值
来源：http://kmj.sxryk.cn

name="${1:-default}"
来源：http://zxl.0kj1m.cn

[R06] 判断命令是否存在
来源：http://oym.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ltv.zhengqikj.top

[R07] if 判断文件
来源：http://njb.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zap.yonumen.top

[R08] 数值比较
来源：http://ibv.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zgz.quarkkingdee.top

[R09] 字符串比较
来源：http://awo.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://byo.sysykeji.top

[R10] 正则匹配
来源：http://grm.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qra.sufxvd.cn

[R11] case 多分支
来源：http://khs.hammf.cn

case "$1" in
来源：http://fzx.ctjpmb.com

start) echo "启动" ;;
来源：http://age.pycfn.com

stop)  echo "停止" ;;
来源：http://gxl.316326.xyz

*)     echo "未知命令" ;;
来源：http://nhd.yueranfly.top

esac
来源：http://dti.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://fld.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://xmw.andypj.xyz

[R13] for 计数循环
来源：http://dlz.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://qbs.tanke756.top

[R14] C 风格 for
来源：http://imq.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ngm.hammf.cn

[R15] while 逐行读文件
来源：http://lpe.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hep.jiagoushi.top

[R16] until 等待条件
来源：http://ygd.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fub.smart0.xyz

[R17] 数组定义与取值
来源：http://yjx.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ise.mhx1999.top

[R18] 遍历数组
来源：http://vkb.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kas.9152youxi.cn

[R19] 数组长度
来源：http://wct.mhx1999.top

echo "${#arr[@]}"
来源：http://gfq.guannengcc.top

[R20] 关联数组（字典）
来源：http://qet.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yke.yj202588.top

[R21] 字符串长度
来源：http://pgp.hcnkem.com

echo "${#s}"
来源：http://tub.ehwqpu.com

[R22] 截取子串
来源：http://gml.cdnleiting.top

echo "${s:0:5}"
来源：http://tyq.ehwqpu.com

[R23] 字符串替换
来源：http://dfo.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://enf.cashguo.top

[R24] 大小写转换
来源：http://lqi.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ecz.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://ewl.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sma.zhoulong.xyz

[R26] 命令替换
来源：http://ujm.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://qjk.jlsjyb.cn

[R27] 算术展开
来源：http://sqn.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://rxr.nanxinkj.top

[R28] 浮点运算
来源：http://jyt.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://ond.yj20258.top

[R29] 定义函数
来源：http://duf.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yff.fehbvm.com

[R30] 函数返回状态码
来源：http://fki.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://vlq.shzxlz.cn

[R31] 局部变量
来源：http://eut.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://otx.aizwys.cn

[R32] 参数个数校验
来源：http://yzh.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vod.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://xsu.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xva.cdnleiting.top

[R34] 退出时清理
来源：http://qwq.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://ijf.sufxvd.cn

[R35] 后台执行并等待
来源：http://ezg.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eho.epnwcf.com

[R36] 并发执行多个任务
来源：http://zgf.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mmt.meibo888.top

[R37] 把输出赋给变量
来源：http://bca.yangfankeji.com

files=$(ls -1)
来源：http://qzi.wangshuangyany.cn

[R38] 管道串联
来源：http://mfs.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://myv.havefunace.top

[R39] 重定向标准输出与错误
来源：http://npj.aizwys.cn

cmd > out.log 2>&1
来源：http://odv.yangfankeji.com

[R40] 追加写日志
来源：http://igz.zhengqikj.top

echo "log" >> out.log
来源：http://eau.shzxlz.cn

[R41] 丢弃输出
来源：http://mbw.birdmap.top

cmd >/dev/null 2>&1
来源：http://zya.hnxiangtu.top

[R42] 输入重定向
来源：http://xlb.zhixingplan.top

wc -l < a.txt
来源：http://xst.vehdjk.com

[R43] 按名字查找文件
来源：http://pxq.haohaochexian.top

find . -name "*.log" -type f
来源：http://gsi.hnqzz.top

[R44] 按修改时间查找
来源：http://osg.52xcode.cn

find . -mtime -7 -type f
来源：http://dqb.yfazqb.com

[R45] 批量删除
来源：http://juj.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://jpe.iojbl.cn

[R46] 递归替换文件内容
来源：http://hpk.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zfv.jqgfzy.top

[R47] sed 单行替换
来源：http://lvx.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://pog.xuanzx.com

[R48] awk 取指定列
来源：http://dys.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://ghi.birdmap.top

[R49] awk 带条件
来源：http://cut.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pca.fktsv.cn

[R50] awk 求和
来源：http://qcx.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ftg.pycfn.com

[R51] 排序去重取前几
来源：http://nmj.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ugx.fzhhl.top

[R52] 统计行数
来源：http://nsr.snrcjt.cn

wc -l a.txt
来源：http://lgg.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://zsa.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aiz.jianghu66.top

[R54] 比较两个文件
来源：http://ksr.zhoulong.xyz

diff a.txt b.txt
来源：http://ruu.0kj1m.cn

[R55] 压缩与解压
来源：http://nkp.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lry.guowangkeji.top

[R56] 远程拷贝
来源：http://xkg.chenzaomai.com

scp file user@host:/path/
来源：http://xdf.ydjk.org.cn

[R57] 远程执行命令
来源：http://mrx.birdmap.top

ssh user@host 'uptime'
来源：http://lvz.jinghuilouyu.cn

[R58] 下载文件
来源：http://zvb.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://evz.guowangkeji.top

[R59] 发 POST JSON
来源：http://wvh.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qgw.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://yyk.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nkd.cqqwz.cn

[R61] 磁盘占用
来源：http://jkr.fktsv.cn

df -h;  du -sh *
来源：http://hpy.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://emn.uphjek.com

du -ah . | sort -rh | head -10
来源：http://utv.ivvv.top

[R63] 内存与进程
来源：http://ycx.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://dss.meibo888.top

[R64] 结束进程
来源：http://obb.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://yrt.zhixingplan.top

[R65] 查看端口占用
来源：http://qoo.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mka.guowangkeji.top

[R66] 定时任务
来源：http://ttq.ybcxt.top

crontab -e;  crontab -l
来源：http://weo.ivvv.top

[R67] 生成随机十六进制串
来源：http://gfx.xziqi.cn

openssl rand -hex 16
来源：http://eis.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://mif.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://ork.birdmap.top

[R69] 生成随机密码
来源：http://oyp.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://lia.hnxiangtu.top

[R70] 时间戳与互转
来源：http://ozc.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://ijw.hammf.cn

[R71] 日期格式化
来源：http://oaj.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ggo.fktsv.cn

[R72] 等待端口就绪
来源：http://ptq.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mdk.jlsjyb.cn

[R73] 分割大日志
来源：http://pif.pycfn.com

split -l 1000 big.log part_
来源：http://ioy.chenzaomai.com

[R74] 批量重命名
来源：http://usf.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vup.tanke756.top

[R75] 导出环境变量
来源：http://wvl.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://vzg.fzhhl.top

[R76] 使用临时文件
来源：http://nip.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hsu.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://omx.hfpthk.cn

read -rp "请输入: " ans
来源：http://mfq.haohaochexian.top

[R78] 交互式菜单
来源：http://vab.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tbz.yuanzhike.top

[R79] 解析命令行选项
来源：http://ofr.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zvp.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://ibm.gzhubu.top

time ./run.sh
来源：http://fdx.hnxiangtu.top

================================================================================
来源：http://lhi.xuetiantiany.cn

S. C / C++ 专题
来源：http://otj.chenlongwang.top

================================================================================
来源：http://wdw.tanke756.top

[S01] C：Hello World
来源：http://wst.jianghu66.top

#include <stdio.h>
来源：http://nbb.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://isj.yfazqb.com

[S02] C：变量与格式化输出
来源：http://ypl.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://sye.hysaishi.cn

[S03] C：读入整数
来源：http://hzf.guannengcc.top

int x; scanf("%d", &x);
来源：http://euv.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://rwz.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://rni.ehwqpu.com

[S05] C：字符串长度
来源：http://qsd.hysaishi.cn

strlen(s)
来源：http://nhr.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://zhw.zhengqikj.top

strcmp(a, b) == 0
来源：http://din.xziqi.cn

[S07] C：数组遍历求和
来源：http://xqa.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cit.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://kux.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xuy.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://iiw.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jem.sysykeji.top

[S10] C：指针与解引用
来源：http://yla.cashguo.top

int *p = &a;  *p = 5;
来源：http://ybr.316326.xyz

[S11] C：逐行读文件
来源：http://unz.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://yim.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ixn.cdnleiting.top

fclose(f);
来源：http://rjj.zhijiandao.cn

[S12] C：写文件
来源：http://mps.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hqg.xuanzx.com

[S13] C：宏定义
来源：http://tiu.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vsx.yangfankeji.com

[S14] C：枚举
来源：http://abp.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://vkr.fktsv.cn

[S15] C：类型转换
来源：http://obg.yuxming.cn

(double) a / b
来源：http://gwi.jinqigufen.top

[S16] C：位操作置位
来源：http://kke.gaohongyu789.top

x |= (1 << 3);
来源：http://miu.hnqzz.top

[S17] C：安全拼接字符串
来源：http://pur.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qoh.chenjidiqi.icu

[S18] C：命令行参数
来源：http://nxk.zhixingplan.top

int main(int argc, char **argv)
来源：http://plf.jianghu66.top

[S19] C：快速排序
来源：http://xom.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://vth.hfpthk.cn

[S20] C：二分查找
来源：http://bjs.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://byp.sxryk.cn

[S21] C：字符类别判断
来源：http://mxu.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mfy.aizwys.cn

[S22] C：字符串转数字
来源：http://kip.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://ove.yfazqb.com

[S23] C：随机数
来源：http://npr.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pwz.cheryme.top

[S24] C：获取本地时间
来源：http://lii.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://weg.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://biw.cashguo.top

memcpy(dst, src, n);
来源：http://fov.jqgfzy.top

[S26] C：内存清零
来源：http://dux.pycfn.com

memset(a, 0, sizeof a);
来源：http://wzq.tarul.cn

[S27] C：定义常量
来源：http://aml.sxryk.cn

const double PI = 3.14159;
来源：http://qjy.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://ego.cucudq.cn

static int counter = 0;
来源：http://rip.hnqzz.top

[S29] C：变参函数
来源：http://hwx.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bnp.sufxvd.cn

[S30] C：头文件保护
来源：http://tti.kuanghao11.cn

#ifndef X_H
来源：http://dlt.jinqigfzy.top

#define X_H
来源：http://glh.jiagoushi.top

#endif
来源：http://pct.cashguo.top

[S31] C++：Hello World
来源：http://swq.snrcjt.cn


<!-- 参考信息 -->