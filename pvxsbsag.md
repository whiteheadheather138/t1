代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mnm.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://psx.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zzp.yfazqb.com

[Q57] 行号
来源：http://ixf.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fnh.yj202588.top

[Q58] 累计求和
来源：http://cwk.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tbm.xinyue.icu

[Q59] 分组内累计
来源：http://vtc.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dci.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://jwa.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wtq.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mok.nanxinkj.top

[Q61] 移动平均
来源：http://xun.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hyz.xinyue.icu

[Q62] 分组占比
来源：http://wly.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rio.ybcxt.top

[Q63] 开启事务
来源：http://soy.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yzw.dianchejie.cn

[Q64] 提交事务
来源：http://nfd.chenjidiqi.icu

COMMIT;
来源：http://efv.yangfankeji.com

[Q65] 回滚事务
来源：http://wjo.jinqigfzy.top

ROLLBACK;
来源：http://yzf.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://nqh.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vla.daria6918.cn

[Q67] 设置隔离级别
来源：http://kxv.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mol.quarkkingdee.top

[Q68] 保存点
来源：http://iha.tanke756.top

SAVEPOINT sp1;
来源：http://cpa.guannengcc.top

ROLLBACK TO sp1;
来源：http://cvi.yangfankeji.com

[Q69] 查看执行计划
来源：http://fvp.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nss.ivvv.top

[Q70] 更新统计信息
来源：http://tvz.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://pbj.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://ixi.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ool.hammf.cn

[Q72] 查看索引
来源：http://ftp.hfpthk.cn

SHOW INDEX FROM users;
来源：http://rpm.jinqigfzy.top

[Q73] 查看表状态
来源：http://dga.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cyd.jqgufenzy.top

[Q74] 强制使用索引
来源：http://dhy.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dui.jyoumei.cn

[Q75] 日期格式化
来源：http://qtl.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wrn.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vne.xylfe.cn

[Q76] 按天统计
来源：http://wpe.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oei.fanxiaobao.xyz

[Q77] 时间加减
来源：http://ccg.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jxv.sxryk.cn

[Q78] 当前时间
来源：http://fwe.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fbx.shuidangran.top

[Q79] 字符串拼接
来源：http://pcu.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://avv.jqgfzy.top

[Q80] 字符串截取
来源：http://haz.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zdz.wangdashe.top

[Q81] 字符串替换
来源：http://ito.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mxg.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://bps.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cyi.zhijiandao.cn

[Q83] 大小写转换
来源：http://kmn.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gdi.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://ast.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://xqj.yj20258888.top

[Q85] 数值取整
来源：http://gwv.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://okh.pycfn.com

[Q86] 读取 JSON 字段
来源：http://akh.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dpw.havefunace.top

[Q87] JSON 字段做条件
来源：http://jnh.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ljf.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://chs.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://byx.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aep.ivvv.top

[Q89] 判断表是否存在
来源：http://xrz.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gpl.yfazqb.com

[Q90] 生成序号列
来源：http://ngg.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sts.epnwcf.com

================================================================================
来源：http://ooq.yuxming.cn

R. Bash 专题
来源：http://pmo.xinyue.icu

================================================================================
来源：http://oyn.fehbvm.com

[R01] shebang 与严格模式
来源：http://jio.jiagoushi.top

#!/usr/bin/env bash
来源：http://iqi.tarul.cn

set -euo pipefail
来源：http://kjj.xziqi.cn

[R02] 变量赋值与使用
来源：http://fim.xinyue.icu

name="Tom"; echo "$name"
来源：http://myd.nanxuanxn.top

[R03] 只读变量
来源：http://zpq.jyoumei.cn

readonly PI=3.14
来源：http://hrz.jianghu66.top

[R04] 位置参数
来源：http://xgk.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://knr.wangshuangyany.cn

[R05] 参数默认值
来源：http://ihi.hfpthk.cn

name="${1:-default}"
来源：http://hhx.yangfankeji.com

[R06] 判断命令是否存在
来源：http://mpr.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://prq.sysykeji.top

[R07] if 判断文件
来源：http://gry.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://puz.jyoumei.cn

[R08] 数值比较
来源：http://kpb.fengsongda.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vuy.pycfn.com

[R09] 字符串比较
来源：http://ydp.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tui.yanxiufei.cn

[R10] 正则匹配
来源：http://nrl.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dwa.nanxuanxn.top

[R11] case 多分支
来源：http://dmx.zhijiandao.cn

case "$1" in
来源：http://kyk.gotoacloud.top

start) echo "启动" ;;
来源：http://fiv.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://jkw.xylfe.cn

*)     echo "未知命令" ;;
来源：http://fcd.tanke756.top

esac
来源：http://ccp.andypj.xyz

[R12] for 遍历文件
来源：http://jtg.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://gmw.hywenlv.cn

[R13] for 计数循环
来源：http://ggx.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://pim.fzhhl.top

[R14] C 风格 for
来源：http://fjz.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xwz.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://cmi.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pjr.52xcode.cn

[R16] until 等待条件
来源：http://zvo.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yfj.fehbvm.com

[R17] 数组定义与取值
来源：http://vhr.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://xff.sysykeji.top

[R18] 遍历数组
来源：http://tbk.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://svi.hywenlv.cn

[R19] 数组长度
来源：http://lmq.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://nij.snrcjt.cn

[R20] 关联数组（字典）
来源：http://epp.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lwe.cucudq.cn

[R21] 字符串长度
来源：http://cuk.yvedp.cn

echo "${#s}"
来源：http://czq.tanke756.top

[R22] 截取子串
来源：http://sxv.jinqigufen.top

echo "${s:0:5}"
来源：http://hcj.daria6918.cn

[R23] 字符串替换
来源：http://hko.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xjc.jyoumei.cn

[R24] 大小写转换
来源：http://hlv.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://qtb.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://sib.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ddj.xziqi.cn

[R26] 命令替换
来源：http://fal.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://rep.feifeiyinyue.top

[R27] 算术展开
来源：http://oqr.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://nig.bjfxy.top

[R28] 浮点运算
来源：http://ofh.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://ddu.jinqigufen.top

[R29] 定义函数
来源：http://jtn.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ngh.nwbrower.top

[R30] 函数返回状态码
来源：http://bfn.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://pkh.hnqzz.top

[R31] 局部变量
来源：http://kps.ivvv.top

f() { local x=1; echo "$x"; }
来源：http://ewt.xinyue.icu

[R32] 参数个数校验
来源：http://qrm.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ilm.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://afp.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zig.aizwys.cn

[R34] 退出时清理
来源：http://spy.shanyushiyangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://ncs.jinqigufen.top

[R35] 后台执行并等待
来源：http://uly.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zra.guannengcc.top

[R36] 并发执行多个任务
来源：http://wza.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://otu.hywenlv.cn

[R37] 把输出赋给变量
来源：http://phx.zycfv.cn

files=$(ls -1)
来源：http://cfm.52xcode.cn

[R38] 管道串联
来源：http://azz.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://wzb.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://bsq.xylfe.cn

cmd > out.log 2>&1
来源：http://anc.shuidangran.top

[R40] 追加写日志
来源：http://ydp.zdbjq.cn

echo "log" >> out.log
来源：http://ijc.yvedp.cn

[R41] 丢弃输出
来源：http://fvc.yonumen.top

cmd >/dev/null 2>&1
来源：http://twn.yvedp.cn

[R42] 输入重定向
来源：http://qkl.birdmap.top

wc -l < a.txt
来源：http://gya.dashuyun.cn

[R43] 按名字查找文件
来源：http://iwy.jqgufenzy.top

find . -name "*.log" -type f
来源：http://jtp.haohaochexian.top

[R44] 按修改时间查找
来源：http://dey.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://elo.yj202588.top

[R45] 批量删除
来源：http://iei.yueranfly.top

find . -name "*.tmp" -delete
来源：http://wvw.gogol.net.cn

[R46] 递归替换文件内容
来源：http://thv.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://daw.jinqigufen.top

[R47] sed 单行替换
来源：http://bzn.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://xyu.yonumen.top

[R48] awk 取指定列
来源：http://slz.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://lta.cqqwz.cn

[R49] awk 带条件
来源：http://lmj.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hym.zhaomingkeji.xyz

[R50] awk 求和
来源：http://yjv.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://mmf.birdmap.top

[R51] 排序去重取前几
来源：http://grp.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://olc.bjfxy.top

[R52] 统计行数
来源：http://pzy.yuanzhike.top

wc -l a.txt
来源：http://fcs.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://cwl.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wet.gzhubu.top

[R54] 比较两个文件
来源：http://okd.ehwqpu.com

diff a.txt b.txt
来源：http://jru.guowangkeji.top

[R55] 压缩与解压
来源：http://hye.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cor.uphjek.com

[R56] 远程拷贝
来源：http://pmy.cdnleiting.top

scp file user@host:/path/
来源：http://uut.jinqigfzy.top

[R57] 远程执行命令
来源：http://wpm.jinqigfzy.top

ssh user@host 'uptime'
来源：http://tvy.pengpengdd.cyou

[R58] 下载文件
来源：http://bvf.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://whk.jiagoushi.top

[R59] 发 POST JSON
来源：http://vjx.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lfk.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://xcb.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vkq.jinqigfzy.top

[R61] 磁盘占用
来源：http://oyn.bjfxy.top

df -h;  du -sh *
来源：http://ndr.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://iaa.yonumen.top

du -ah . | sort -rh | head -10
来源：http://sfj.9152youxi.cn

[R63] 内存与进程
来源：http://dlo.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://hnp.yuxming.cn

[R64] 结束进程
来源：http://xew.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://vwb.wangshuangyany.cn

[R65] 查看端口占用
来源：http://dlq.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eur.tianlin.xyz

[R66] 定时任务
来源：http://pvc.yuxming.cn

crontab -e;  crontab -l
来源：http://lpz.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://sht.vehdjk.com

openssl rand -hex 16
来源：http://xmx.jqgufenzy.top

[R68] 计算文件校验值
来源：http://cio.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://xbh.cqqwz.cn

[R69] 生成随机密码
来源：http://vwk.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://obl.wangdashe.top

[R70] 时间戳与互转
来源：http://bls.pycfn.com

date +%s;  date -d @1700000000
来源：http://afr.hnqzz.top

[R71] 日期格式化
来源：http://lvw.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://noz.hnxiangtu.top

[R72] 等待端口就绪
来源：http://fyu.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gyn.dashuyun.cn

[R73] 分割大日志
来源：http://idt.aizwys.cn

split -l 1000 big.log part_
来源：http://ast.316326.xyz

[R74] 批量重命名
来源：http://bta.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wyk.kuanghao11.cn

[R75] 导出环境变量
来源：http://ejc.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://zbx.cheryme.top

[R76] 使用临时文件
来源：http://bnu.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rra.zdbjq.cn

[R77] 读取用户输入
来源：http://fto.zhoulong.xyz

read -rp "请输入: " ans
来源：http://ijl.hammf.cn

[R78] 交互式菜单
来源：http://xab.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://blq.hesvh.cn

[R79] 解析命令行选项
来源：http://gsu.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qfx.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://rfh.bbcook.cn

time ./run.sh
来源：http://ukz.c1oappe.top

================================================================================
来源：http://tkb.hnxiangtu.top

S. C / C++ 专题
来源：http://juz.shzxlz.cn

================================================================================
来源：http://cor.sufxvd.cn

[S01] C：Hello World
来源：http://qnq.vqdsnc.cn

#include <stdio.h>
来源：http://jeg.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://evo.uphjek.com

[S02] C：变量与格式化输出
来源：http://ftg.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://wcm.cucudq.cn

[S03] C：读入整数
来源：http://tbl.zhengqikj.top

int x; scanf("%d", &x);
来源：http://izs.daria6918.cn

[S04] C：字符串复制
来源：http://jrx.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://aum.jianghu66.top

[S05] C：字符串长度
来源：http://fyj.iojbl.cn

strlen(s)
来源：http://hsi.daxiang520.top

[S06] C：字符串比较
来源：http://pos.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://ecu.zdqjudy.top

[S07] C：数组遍历求和
来源：http://pgi.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://etn.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://uue.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xcx.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://lvr.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ewk.yj202588.top

[S10] C：指针与解引用
来源：http://gtq.pycfn.com

int *p = &a;  *p = 5;
来源：http://uhv.hcnkem.com

[S11] C：逐行读文件
来源：http://qnk.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://fen.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://xyc.yongpay.top

fclose(f);
来源：http://bpo.epnwcf.com

[S12] C：写文件
来源：http://kfa.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tyw.hesvh.cn

[S13] C：宏定义
来源：http://wux.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tad.sxryk.cn

[S14] C：枚举
来源：http://rey.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://bex.yuxming.cn

[S15] C：类型转换
来源：http://bjw.jinyuanbaomall.cn

(double) a / b
来源：http://ztk.gotoacloud.top

[S16] C：位操作置位
来源：http://xcv.birdmap.top

x |= (1 << 3);
来源：http://wmp.andypj.xyz

[S17] C：安全拼接字符串
来源：http://lif.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yvw.jinqigufen.top

[S18] C：命令行参数
来源：http://woo.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://prh.cqqwz.cn

[S19] C：快速排序
来源：http://nxo.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yhh.yuanzhike.top

[S20] C：二分查找
来源：http://mnx.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ajb.tarul.cn

[S21] C：字符类别判断
来源：http://ced.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lbc.dashuyun.cn

[S22] C：字符串转数字
来源：http://aox.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xse.svipenyu.cn

[S23] C：随机数
来源：http://cle.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tro.xuanzx.com

[S24] C：获取本地时间
来源：http://nii.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mjy.tanke756.top

[S25] C：内存拷贝
来源：http://jpo.gogol.net.cn

memcpy(dst, src, n);
来源：http://cbu.meibo888.top

[S26] C：内存清零
来源：http://gju.meibo888.top


<!-- 参考信息 -->