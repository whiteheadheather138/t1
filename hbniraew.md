代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lzg.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://wxi.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cdw.bjfxy.top

[Q57] 行号
来源：http://ldh.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pmc.ctjpmb.com

[Q58] 累计求和
来源：http://sxx.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://phl.zhijiandao.cn

[Q59] 分组内累计
来源：http://iiv.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ckg.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://ldy.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://swc.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ztw.cashguo.top

[Q61] 移动平均
来源：http://aof.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pat.gotoacloud.top

[Q62] 分组占比
来源：http://kus.guowangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oas.shuidangran.top

[Q63] 开启事务
来源：http://otu.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rlx.yangfankeji.com

[Q64] 提交事务
来源：http://buj.fengsongda.top

COMMIT;
来源：http://klu.jianghu66.top

[Q65] 回滚事务
来源：http://bkn.bjfxy.top

ROLLBACK;
来源：http://fcl.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://wyg.mhx1999.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://omt.ybcxt.top

[Q67] 设置隔离级别
来源：http://tqu.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cwo.yonumen.top

[Q68] 保存点
来源：http://nkc.zhijiandao.cn

SAVEPOINT sp1;
来源：http://ikg.xylfe.cn

ROLLBACK TO sp1;
来源：http://cso.daria6918.cn

[Q69] 查看执行计划
来源：http://yyl.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xma.c1oappe.top

[Q70] 更新统计信息
来源：http://jnl.fktsv.cn

ANALYZE TABLE users;
来源：http://pdc.smart0.xyz

[Q71] 查看建表语句
来源：http://hmw.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://smn.cqqwz.cn

[Q72] 查看索引
来源：http://lek.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://qey.chenjidiqi.icu

[Q73] 查看表状态
来源：http://xsl.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vab.fengsongda.top

[Q74] 强制使用索引
来源：http://xpe.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cbt.sweek.top

[Q75] 日期格式化
来源：http://knk.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://frp.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jvz.jiagoushi.top

[Q76] 按天统计
来源：http://ear.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ibo.shuidangran.top

[Q77] 时间加减
来源：http://cyi.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dnb.dashuyun.cn

[Q78] 当前时间
来源：http://tut.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://joh.fehbvm.com

[Q79] 字符串拼接
来源：http://bbr.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iyc.pengpengdd.cyou

[Q80] 字符串截取
来源：http://qxl.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pyz.52xcode.cn

[Q81] 字符串替换
来源：http://izp.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uep.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://gws.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yer.jqgufenzy.top

[Q83] 大小写转换
来源：http://dgr.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://phl.fzhhl.top

[Q84] 去除首尾空格
来源：http://anm.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://mck.hesvh.cn

[Q85] 数值取整
来源：http://izx.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gqb.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://sor.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fox.c1oappe.top

[Q87] JSON 字段做条件
来源：http://ecw.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eim.yj202588.top

[Q88] 行转列（条件聚合）
来源：http://qip.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kmm.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ain.yfazqb.com

[Q89] 判断表是否存在
来源：http://xik.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jcl.hammf.cn

[Q90] 生成序号列
来源：http://roo.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wge.vqdsnc.cn

================================================================================
来源：http://tar.tarul.cn

R. Bash 专题
来源：http://voq.zdbjq.cn

================================================================================
来源：http://ink.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://syz.bbcook.cn

#!/usr/bin/env bash
来源：http://cze.zhoulong.xyz

set -euo pipefail
来源：http://cri.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://gyp.redwolf501.top

name="Tom"; echo "$name"
来源：http://xwg.chenjidiqi.icu

[R03] 只读变量
来源：http://ctt.316326.xyz

readonly PI=3.14
来源：http://gia.52xcode.cn

[R04] 位置参数
来源：http://vly.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yyb.hnxiangtu.top

[R05] 参数默认值
来源：http://kmr.bjfxy.top

name="${1:-default}"
来源：http://fpl.andypj.xyz

[R06] 判断命令是否存在
来源：http://hya.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kpx.sweek.top

[R07] if 判断文件
来源：http://wwq.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mni.daria6918.cn

[R08] 数值比较
来源：http://yfx.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bta.ivvv.top

[R09] 字符串比较
来源：http://kfg.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iau.yuxming.cn

[R10] 正则匹配
来源：http://skj.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zar.sxryk.cn

[R11] case 多分支
来源：http://kts.smart0.xyz

case "$1" in
来源：http://fgx.yanxiufei.cn

start) echo "启动" ;;
来源：http://icu.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://etd.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://zwz.jianghu66.top

esac
来源：http://vdm.hywenlv.cn

[R12] for 遍历文件
来源：http://djo.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://ewl.birdmap.top

[R13] for 计数循环
来源：http://biz.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://kwl.hesvh.cn

[R14] C 风格 for
来源：http://fuj.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rlf.hesvh.cn

[R15] while 逐行读文件
来源：http://llv.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://okd.kuanghao11.cn

[R16] until 等待条件
来源：http://bfn.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gel.nwbrower.top

[R17] 数组定义与取值
来源：http://yyi.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kgd.shzxlz.cn

[R18] 遍历数组
来源：http://dho.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://knm.zhoulong.xyz

[R19] 数组长度
来源：http://nkd.birdmap.top

echo "${#arr[@]}"
来源：http://nxu.nanxinkj.top

[R20] 关联数组（字典）
来源：http://dgj.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yyf.cashguo.top

[R21] 字符串长度
来源：http://ltd.epnwcf.com

echo "${#s}"
来源：http://lum.jinqigufen.top

[R22] 截取子串
来源：http://zlg.yangfankeji.com

echo "${s:0:5}"
来源：http://eyu.nwbrower.top

[R23] 字符串替换
来源：http://lfk.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cmf.tian-w.cn

[R24] 大小写转换
来源：http://zhp.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://miv.ydzc1.top

[R25] 去后缀 / 去前缀
来源：http://qdw.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://dea.fanxiaobao.xyz

[R26] 命令替换
来源：http://bwc.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://tji.yj202588.top

[R27] 算术展开
来源：http://hdx.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://wnu.shangyingyoupin.top

[R28] 浮点运算
来源：http://nbs.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://zyd.ybcxt.top

[R29] 定义函数
来源：http://ntp.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fsl.mhx1999.top

[R30] 函数返回状态码
来源：http://eio.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://jwm.jyoumei.cn

[R31] 局部变量
来源：http://rpe.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://kvl.yueranfly.top

[R32] 参数个数校验
来源：http://ywi.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://olr.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://mmf.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://boj.fehbvm.com

[R34] 退出时清理
来源：http://whd.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xjj.tian-w.cn

[R35] 后台执行并等待
来源：http://lqt.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://xhm.aibaodan.cn

[R36] 并发执行多个任务
来源：http://clv.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lft.jyoumei.cn

[R37] 把输出赋给变量
来源：http://lau.yuxming.cn

files=$(ls -1)
来源：http://sxy.dianchejie.cn

[R38] 管道串联
来源：http://hha.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://lcl.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://jxo.havefunace.top

cmd > out.log 2>&1
来源：http://zze.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://vhh.wangdashe.top

echo "log" >> out.log
来源：http://yra.vehdjk.com

[R41] 丢弃输出
来源：http://ykc.gzhubu.top

cmd >/dev/null 2>&1
来源：http://gka.chenjidiqi.icu

[R42] 输入重定向
来源：http://evu.hnxiangtu.top

wc -l < a.txt
来源：http://mmy.iojbl.cn

[R43] 按名字查找文件
来源：http://eed.tanke756.top

find . -name "*.log" -type f
来源：http://llj.snrcjt.cn

[R44] 按修改时间查找
来源：http://erj.52xcode.cn

find . -mtime -7 -type f
来源：http://tug.jiagoushi.top

[R45] 批量删除
来源：http://sqy.cheryme.top

find . -name "*.tmp" -delete
来源：http://itm.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://yzb.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ecx.yonumen.top

[R47] sed 单行替换
来源：http://bxl.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tga.nwbrower.top

[R48] awk 取指定列
来源：http://zff.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://ela.ivvv.top

[R49] awk 带条件
来源：http://zbi.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tog.birdmap.top

[R50] awk 求和
来源：http://wbr.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://pcz.wangdashe.top

[R51] 排序去重取前几
来源：http://xwo.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fyd.xinyue.icu

[R52] 统计行数
来源：http://cim.zdbjq.cn

wc -l a.txt
来源：http://szb.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://oby.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kci.vehdjk.com

[R54] 比较两个文件
来源：http://lhw.shzxlz.cn

diff a.txt b.txt
来源：http://uzz.epnwcf.com

[R55] 压缩与解压
来源：http://ggw.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://llx.fzhhl.top

[R56] 远程拷贝
来源：http://tha.vqdsnc.cn

scp file user@host:/path/
来源：http://lpm.zhijiandao.cn

[R57] 远程执行命令
来源：http://ibf.snrcjt.cn

ssh user@host 'uptime'
来源：http://zak.cheryme.top

[R58] 下载文件
来源：http://omj.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://khi.dashuyun.cn

[R59] 发 POST JSON
来源：http://bug.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wbx.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://kst.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wmj.fzhhl.top

[R61] 磁盘占用
来源：http://uom.shuidangran.top

df -h;  du -sh *
来源：http://wtx.ehwqpu.com

[R62] 找最占空间的文件
来源：http://nzx.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://ncr.hysaishi.cn

[R63] 内存与进程
来源：http://oxa.yj20258.top

free -h;  ps aux | grep nginx
来源：http://ioj.hnxiangtu.top

[R64] 结束进程
来源：http://rni.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://iea.ydjk.org.cn

[R65] 查看端口占用
来源：http://nww.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tyo.snrcjt.cn

[R66] 定时任务
来源：http://vso.yuanzhike.top

crontab -e;  crontab -l
来源：http://dja.wangdashe.top

[R67] 生成随机十六进制串
来源：http://hxp.sweek.top

openssl rand -hex 16
来源：http://kkr.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://rdt.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://lva.pengpengdd.cyou

[R69] 生成随机密码
来源：http://zto.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://rly.wangdashe.top

[R70] 时间戳与互转
来源：http://aqn.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://peu.yfazqb.com

[R71] 日期格式化
来源：http://jxa.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pfe.zycfv.cn

[R72] 等待端口就绪
来源：http://rpz.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aoc.zhijiandao.cn

[R73] 分割大日志
来源：http://qrs.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://xkj.guowangkeji.top

[R74] 批量重命名
来源：http://six.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dao.vehdjk.com

[R75] 导出环境变量
来源：http://rfh.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://shc.hywenlv.cn

[R76] 使用临时文件
来源：http://bxj.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hzi.feifeiyinyue.top

[R77] 读取用户输入
来源：http://xdc.0kj1m.cn

read -rp "请输入: " ans
来源：http://aku.hfpthk.cn

[R78] 交互式菜单
来源：http://klb.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fkp.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://pgn.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vgv.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://qvc.vqdsnc.cn

time ./run.sh
来源：http://bhx.chenlongwang.top

================================================================================
来源：http://dhl.yj20258.top

S. C / C++ 专题
来源：http://ugw.yj202588.top

================================================================================
来源：http://sbf.feifeiyinyue.top

[S01] C：Hello World
来源：http://iue.tanke756.top

#include <stdio.h>
来源：http://usw.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://jup.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://fth.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://opz.cheryme.top

[S03] C：读入整数
来源：http://eww.gzhubu.top

int x; scanf("%d", &x);
来源：http://lqq.tanke756.top

[S04] C：字符串复制
来源：http://nqz.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://ebd.sysykeji.top

[S05] C：字符串长度
来源：http://mje.cucudq.cn

strlen(s)
来源：http://wsn.kuanghao11.cn

[S06] C：字符串比较
来源：http://cyf.pycfn.com

strcmp(a, b) == 0
来源：http://vrl.jiagoushi.top

[S07] C：数组遍历求和
来源：http://qgs.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ecb.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://pvz.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kmg.birdmap.top

[S09] C：结构体定义与初始化
来源：http://mkg.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ias.fzhhl.top

[S10] C：指针与解引用
来源：http://uae.vehdjk.com

int *p = &a;  *p = 5;
来源：http://cfc.yj20258.top

[S11] C：逐行读文件
来源：http://qsu.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://bwh.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://jfw.fanxiaobao.xyz

fclose(f);
来源：http://odq.yuxming.cn

[S12] C：写文件
来源：http://wic.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pfp.birdmap.top

[S13] C：宏定义
来源：http://wls.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://khv.shanyushiyangkeji.top

[S14] C：枚举
来源：http://pjj.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://fas.sysykeji.top

[S15] C：类型转换
来源：http://rhc.cheryme.top

(double) a / b
来源：http://gsx.zycfv.cn

[S16] C：位操作置位
来源：http://xgo.meibo888.top

x |= (1 << 3);
来源：http://jos.shuidangran.top

[S17] C：安全拼接字符串
来源：http://vaa.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ivf.aibaodan.cn

[S18] C：命令行参数
来源：http://gyd.ybcxt.top

int main(int argc, char **argv)
来源：http://hch.shuidangran.top

[S19] C：快速排序
来源：http://odu.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rsb.jinghuilouyu.cn

[S20] C：二分查找
来源：http://kyf.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zsv.mhx1999.top

[S21] C：字符类别判断
来源：http://ihw.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hcw.c1oappe.top

[S22] C：字符串转数字
来源：http://tbl.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://zrc.daria6918.cn

[S23] C：随机数
来源：http://oty.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wjr.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://oqk.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nns.sufxvd.cn

[S25] C：内存拷贝
来源：http://yuj.yj202588.top

memcpy(dst, src, n);
来源：http://mdw.yj20258.top

[S26] C：内存清零
来源：http://njq.hammf.cn


<!-- 参考信息 -->